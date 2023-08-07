# Comparing `tmp/retakesearch-py-2.2.4.tar.gz` & `tmp/retakesearch-py-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-py-2.2.4.tar", last modified: Mon Aug  7 22:43:39 2023, max compression
+gzip compressed data, was "retakesearch-py-2.2.5.tar", last modified: Mon Aug  7 22:45:26 2023, max compression
```

## Comparing `retakesearch-py-2.2.4.tar` & `retakesearch-py-2.2.5.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.022842 retakesearch-py-2.2.4/
--rw-r--r--   0 mingying   (501) staff       (20)      144 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/AUTHORS
--rw-r--r--   0 mingying   (501) staff       (20)     8426 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/CONTRIBUTING.md
--rw-r--r--   0 mingying   (501) staff       (20)    11356 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/LICENSE.txt
--rw-r--r--   0 mingying   (501) staff       (20)      262 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/MANIFEST.in
--rw-r--r--   0 mingying   (501) staff       (20)      257 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/NOTICE.txt
--rw-r--r--   0 mingying   (501) staff       (20)     5636 2023-08-07 22:43:39.022909 retakesearch-py-2.2.4/PKG-INFO
--rw-r--r--   0 mingying   (501) staff       (20)     3792 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/README.md
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.000799 retakesearch-py-2.2.4/opensearchpy/
--rw-r--r--   0 mingying   (501) staff       (20)     6160 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     6727 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/__init__.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.001868 retakesearch-py-2.2.4/opensearchpy/_async/
--rw-r--r--   0 mingying   (501) staff       (20)     1068 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     2006 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/_extra_imports.py
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.005906 retakesearch-py-2.2.4/opensearchpy/_async/client/
--rw-r--r--   0 mingying   (501) staff       (20)    85442 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)    47018 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    29940 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/cat.py
--rw-r--r--   0 mingying   (501) staff       (20)    22836 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/cat.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    17123 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/cluster.py
--rw-r--r--   0 mingying   (501) staff       (20)    14830 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/cluster.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     3410 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/dangling_indices.py
--rw-r--r--   0 mingying   (501) staff       (20)     3762 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/dangling_indices.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2294 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/features.py
--rw-r--r--   0 mingying   (501) staff       (20)     2715 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/features.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    70997 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/indices.py
--rw-r--r--   0 mingying   (501) staff       (20)    53603 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/indices.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5076 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/ingest.py
--rw-r--r--   0 mingying   (501) staff       (20)     5984 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/ingest.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     7921 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/nodes.py
--rw-r--r--   0 mingying   (501) staff       (20)     5859 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/nodes.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1967 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/plugins.py
--rw-r--r--   0 mingying   (501) staff       (20)      623 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/plugins.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1363 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/remote.py
--rw-r--r--   0 mingying   (501) staff       (20)     1793 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/remote.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    15136 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/snapshot.py
--rw-r--r--   0 mingying   (501) staff       (20)    12322 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/snapshot.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4976 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/tasks.py
--rw-r--r--   0 mingying   (501) staff       (20)     3902 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/tasks.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1235 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/utils.py
--rw-r--r--   0 mingying   (501) staff       (20)     1660 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/client/utils.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1715 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/compat.py
--rw-r--r--   0 mingying   (501) staff       (20)     1142 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/compat.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.008280 retakesearch-py-2.2.4/opensearchpy/_async/helpers/
--rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)    17605 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/actions.py
--rw-r--r--   0 mingying   (501) staff       (20)     3705 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/actions.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    16308 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/document.py
--rw-r--r--   0 mingying   (501) staff       (20)      463 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/document.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5956 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/faceted_search.py
--rw-r--r--   0 mingying   (501) staff       (20)      318 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/faceted_search.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    23606 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/index.py
--rw-r--r--   0 mingying   (501) staff       (20)      348 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/index.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5472 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/mapping.py
--rw-r--r--   0 mingying   (501) staff       (20)      312 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/mapping.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    17058 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/search.py
--rw-r--r--   0 mingying   (501) staff       (20)      398 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/search.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1314 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/test.py
--rw-r--r--   0 mingying   (501) staff       (20)      571 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/test.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4675 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/update_by_query.py
--rw-r--r--   0 mingying   (501) staff       (20)      368 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/helpers/update_by_query.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    14193 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/http_aiohttp.py
--rw-r--r--   0 mingying   (501) staff       (20)     2621 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/http_aiohttp.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.009373 retakesearch-py-2.2.4/opensearchpy/_async/plugins/
--rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/plugins/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/plugins/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     6548 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/plugins/alerting.py
--rw-r--r--   0 mingying   (501) staff       (20)     2619 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/plugins/alerting.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4959 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/plugins/index_management.py
--rw-r--r--   0 mingying   (501) staff       (20)     2036 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/plugins/index_management.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    21802 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/plugins/security.py
--rw-r--r--   0 mingying   (501) staff       (20)     7330 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/plugins/security.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    18066 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/transport.py
--rw-r--r--   0 mingying   (501) staff       (20)     3390 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/_async/transport.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1094 2023-08-07 22:43:33.000000 retakesearch-py-2.2.4/opensearchpy/_version.py
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.012885 retakesearch-py-2.2.4/opensearchpy/client/
--rw-r--r--   0 mingying   (501) staff       (20)    84926 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)    46696 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    29568 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/cat.py
--rw-r--r--   0 mingying   (501) staff       (20)    22704 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/cat.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    16943 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/cluster.py
--rw-r--r--   0 mingying   (501) staff       (20)    14740 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/cluster.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     3374 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/dangling_indices.py
--rw-r--r--   0 mingying   (501) staff       (20)     3744 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/dangling_indices.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2270 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/features.py
--rw-r--r--   0 mingying   (501) staff       (20)     2703 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/features.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    71619 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/indices.py
--rw-r--r--   0 mingying   (501) staff       (20)    53267 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/indices.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5004 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/ingest.py
--rw-r--r--   0 mingying   (501) staff       (20)     5948 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/ingest.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     7861 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/nodes.py
--rw-r--r--   0 mingying   (501) staff       (20)     5829 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/nodes.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2020 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/plugins.py
--rw-r--r--   0 mingying   (501) staff       (20)      613 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/plugins.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1351 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/remote.py
--rw-r--r--   0 mingying   (501) staff       (20)     1787 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/remote.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    14992 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/snapshot.py
--rw-r--r--   0 mingying   (501) staff       (20)    12250 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/snapshot.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4940 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/tasks.py
--rw-r--r--   0 mingying   (501) staff       (20)     3884 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/tasks.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     6925 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/utils.py
--rw-r--r--   0 mingying   (501) staff       (20)     1988 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/client/utils.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2403 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/compat.py
--rw-r--r--   0 mingying   (501) staff       (20)     1941 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/compat.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.014956 retakesearch-py-2.2.4/opensearchpy/connection/
--rw-r--r--   0 mingying   (501) staff       (20)     1605 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     1395 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     3813 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/async_connections.py
--rw-r--r--   0 mingying   (501) staff       (20)      308 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/async_connections.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    11045 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/base.py
--rw-r--r--   0 mingying   (501) staff       (20)     3514 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/base.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4419 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/connections.py
--rw-r--r--   0 mingying   (501) staff       (20)     1154 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/connections.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    10568 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/http_async.py
--rw-r--r--   0 mingying   (501) staff       (20)     1267 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/http_async.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     8719 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/http_requests.py
--rw-r--r--   0 mingying   (501) staff       (20)     1761 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/http_requests.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    10657 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/http_urllib3.py
--rw-r--r--   0 mingying   (501) staff       (20)     2191 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/http_urllib3.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2048 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/pooling.py
--rw-r--r--   0 mingying   (501) staff       (20)     1332 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection/pooling.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    11778 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection_pool.py
--rw-r--r--   0 mingying   (501) staff       (20)     3198 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/connection_pool.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5960 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/exceptions.py
--rw-r--r--   0 mingying   (501) staff       (20)     2275 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/exceptions.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.019999 retakesearch-py-2.2.4/opensearchpy/helpers/
--rw-r--r--   0 mingying   (501) staff       (20)     1929 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     2139 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    24406 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/actions.py
--rw-r--r--   0 mingying   (501) staff       (20)     4186 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/actions.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     9849 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/aggs.py
--rw-r--r--   0 mingying   (501) staff       (20)     3487 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/aggs.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     8525 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/analysis.py
--rw-r--r--   0 mingying   (501) staff       (20)     2161 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/analysis.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1866 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/asyncsigner.py
--rw-r--r--   0 mingying   (501) staff       (20)      595 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/asyncsigner.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    18613 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/document.py
--rw-r--r--   0 mingying   (501) staff       (20)     1347 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/document.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     1487 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/errors.py
--rw-r--r--   0 mingying   (501) staff       (20)     1378 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/errors.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    13797 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/faceted_search.py
--rw-r--r--   0 mingying   (501) staff       (20)     1374 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/faceted_search.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    14196 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/field.py
--rw-r--r--   0 mingying   (501) staff       (20)     2257 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/field.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     3857 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/function.py
--rw-r--r--   0 mingying   (501) staff       (20)     1459 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/function.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    22993 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/index.py
--rw-r--r--   0 mingying   (501) staff       (20)     1127 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/index.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     7960 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/mapping.py
--rw-r--r--   0 mingying   (501) staff       (20)     1155 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/mapping.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    12671 2023-08-07 20:06:34.000000 retakesearch-py-2.2.4/opensearchpy/helpers/query.py
--rw-r--r--   0 mingying   (501) staff       (20)     2952 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/query.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.020696 retakesearch-py-2.2.4/opensearchpy/helpers/response/
--rw-r--r--   0 mingying   (501) staff       (20)     4409 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/response/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     1205 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/response/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2946 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/response/aggs.py
--rw-r--r--   0 mingying   (501) staff       (20)     1315 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/response/aggs.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2161 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/response/hit.py
--rw-r--r--   0 mingying   (501) staff       (20)     1124 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/response/hit.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    27545 2023-08-07 20:54:12.000000 retakesearch-py-2.2.4/opensearchpy/helpers/search.py
--rw-r--r--   0 mingying   (501) staff       (20)     1313 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/search.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2900 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/signer.py
--rw-r--r--   0 mingying   (501) staff       (20)     3459 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/test.py
--rw-r--r--   0 mingying   (501) staff       (20)     1579 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/test.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     5344 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/update_by_query.py
--rw-r--r--   0 mingying   (501) staff       (20)     1132 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/update_by_query.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    19065 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/utils.py
--rw-r--r--   0 mingying   (501) staff       (20)     1238 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/utils.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     2868 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/wrappers.py
--rw-r--r--   0 mingying   (501) staff       (20)     1125 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/helpers/wrappers.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.021756 retakesearch-py-2.2.4/opensearchpy/plugins/
--rw-r--r--   0 mingying   (501) staff       (20)      281 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/plugins/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/plugins/__init__.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     6391 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/plugins/alerting.py
--rw-r--r--   0 mingying   (501) staff       (20)     2396 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/plugins/alerting.pyi
--rw-r--r--   0 mingying   (501) staff       (20)     4863 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/plugins/index_management.py
--rw-r--r--   0 mingying   (501) staff       (20)     1988 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/plugins/index_management.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    21208 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/plugins/security.py
--rw-r--r--   0 mingying   (501) staff       (20)     7652 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/plugins/security.pyi
--rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/py.typed
--rw-r--r--   0 mingying   (501) staff       (20)     6226 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/serializer.py
--rw-r--r--   0 mingying   (501) staff       (20)     1876 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/serializer.pyi
--rw-r--r--   0 mingying   (501) staff       (20)    18470 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/transport.py
--rw-r--r--   0 mingying   (501) staff       (20)     3507 2023-07-23 18:55:25.000000 retakesearch-py-2.2.4/opensearchpy/transport.pyi
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:43:39.022719 retakesearch-py-2.2.4/retakesearch_py.egg-info/
--rw-r--r--   0 mingying   (501) staff       (20)     5636 2023-08-07 22:43:38.000000 retakesearch-py-2.2.4/retakesearch_py.egg-info/PKG-INFO
--rw-r--r--   0 mingying   (501) staff       (20)     6173 2023-08-07 22:43:38.000000 retakesearch-py-2.2.4/retakesearch_py.egg-info/SOURCES.txt
--rw-r--r--   0 mingying   (501) staff       (20)        1 2023-08-07 22:43:38.000000 retakesearch-py-2.2.4/retakesearch_py.egg-info/dependency_links.txt
--rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-23 18:56:34.000000 retakesearch-py-2.2.4/retakesearch_py.egg-info/not-zip-safe
--rw-r--r--   0 mingying   (501) staff       (20)      454 2023-08-07 22:43:38.000000 retakesearch-py-2.2.4/retakesearch_py.egg-info/requires.txt
--rw-r--r--   0 mingying   (501) staff       (20)       13 2023-08-07 22:43:38.000000 retakesearch-py-2.2.4/retakesearch_py.egg-info/top_level.txt
--rw-r--r--   0 mingying   (501) staff       (20)      280 2023-08-07 22:43:39.023138 retakesearch-py-2.2.4/setup.cfg
--rw-r--r--   0 mingying   (501) staff       (20)     4775 2023-07-31 22:41:58.000000 retakesearch-py-2.2.4/setup.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.965873 retakesearch-py-2.2.5/
+-rw-r--r--   0 mingying   (501) staff       (20)      144 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/AUTHORS
+-rw-r--r--   0 mingying   (501) staff       (20)     8426 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/CONTRIBUTING.md
+-rw-r--r--   0 mingying   (501) staff       (20)    11356 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/LICENSE.txt
+-rw-r--r--   0 mingying   (501) staff       (20)      262 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/MANIFEST.in
+-rw-r--r--   0 mingying   (501) staff       (20)      257 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/NOTICE.txt
+-rw-r--r--   0 mingying   (501) staff       (20)     5636 2023-08-07 22:45:26.965950 retakesearch-py-2.2.5/PKG-INFO
+-rw-r--r--   0 mingying   (501) staff       (20)     3792 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/README.md
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.937527 retakesearch-py-2.2.5/opensearchpy/
+-rw-r--r--   0 mingying   (501) staff       (20)     6160 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     6727 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/__init__.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.939395 retakesearch-py-2.2.5/opensearchpy/_async/
+-rw-r--r--   0 mingying   (501) staff       (20)     1068 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2006 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/_extra_imports.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.944831 retakesearch-py-2.2.5/opensearchpy/_async/client/
+-rw-r--r--   0 mingying   (501) staff       (20)    85442 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)    47018 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    29940 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/cat.py
+-rw-r--r--   0 mingying   (501) staff       (20)    22836 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/cat.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    17123 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/cluster.py
+-rw-r--r--   0 mingying   (501) staff       (20)    14830 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/cluster.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     3410 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/dangling_indices.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3762 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/dangling_indices.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2294 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/features.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2715 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/features.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    70997 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/indices.py
+-rw-r--r--   0 mingying   (501) staff       (20)    53603 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/indices.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5076 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/ingest.py
+-rw-r--r--   0 mingying   (501) staff       (20)     5984 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/ingest.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     7921 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/nodes.py
+-rw-r--r--   0 mingying   (501) staff       (20)     5859 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/nodes.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1967 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/plugins.py
+-rw-r--r--   0 mingying   (501) staff       (20)      623 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/plugins.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1363 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/remote.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1793 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/remote.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    15136 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/snapshot.py
+-rw-r--r--   0 mingying   (501) staff       (20)    12322 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/snapshot.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4976 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/tasks.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3902 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/tasks.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1235 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/utils.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1660 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/client/utils.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1715 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/compat.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1142 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/compat.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.948061 retakesearch-py-2.2.5/opensearchpy/_async/helpers/
+-rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)    17605 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/actions.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3705 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/actions.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    16308 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/document.py
+-rw-r--r--   0 mingying   (501) staff       (20)      463 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/document.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5956 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/faceted_search.py
+-rw-r--r--   0 mingying   (501) staff       (20)      318 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/faceted_search.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    23606 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/index.py
+-rw-r--r--   0 mingying   (501) staff       (20)      348 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/index.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5472 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/mapping.py
+-rw-r--r--   0 mingying   (501) staff       (20)      312 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/mapping.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    17058 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/search.py
+-rw-r--r--   0 mingying   (501) staff       (20)      398 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/search.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1314 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/test.py
+-rw-r--r--   0 mingying   (501) staff       (20)      571 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/test.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4675 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/update_by_query.py
+-rw-r--r--   0 mingying   (501) staff       (20)      368 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/helpers/update_by_query.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    14193 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/http_aiohttp.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2621 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/http_aiohttp.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.949378 retakesearch-py-2.2.5/opensearchpy/_async/plugins/
+-rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/plugins/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/plugins/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     6548 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/plugins/alerting.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2619 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/plugins/alerting.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4959 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/plugins/index_management.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2036 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/plugins/index_management.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    21802 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/plugins/security.py
+-rw-r--r--   0 mingying   (501) staff       (20)     7330 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/plugins/security.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    18066 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/transport.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3390 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/_async/transport.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1094 2023-08-07 22:45:12.000000 retakesearch-py-2.2.5/opensearchpy/_version.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.954244 retakesearch-py-2.2.5/opensearchpy/client/
+-rw-r--r--   0 mingying   (501) staff       (20)    84926 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)    46696 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    29568 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/cat.py
+-rw-r--r--   0 mingying   (501) staff       (20)    22704 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/cat.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    16943 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/cluster.py
+-rw-r--r--   0 mingying   (501) staff       (20)    14740 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/cluster.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     3374 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/dangling_indices.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3744 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/dangling_indices.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2270 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/features.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2703 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/features.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    71619 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/indices.py
+-rw-r--r--   0 mingying   (501) staff       (20)    53267 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/indices.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5004 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/ingest.py
+-rw-r--r--   0 mingying   (501) staff       (20)     5948 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/ingest.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     7861 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/nodes.py
+-rw-r--r--   0 mingying   (501) staff       (20)     5829 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/nodes.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2020 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/plugins.py
+-rw-r--r--   0 mingying   (501) staff       (20)      613 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/plugins.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1351 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/remote.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1787 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/remote.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    14992 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/snapshot.py
+-rw-r--r--   0 mingying   (501) staff       (20)    12250 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/snapshot.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4940 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/tasks.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3884 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/tasks.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     6925 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/utils.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1988 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/client/utils.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2403 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/compat.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1941 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/compat.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.956501 retakesearch-py-2.2.5/opensearchpy/connection/
+-rw-r--r--   0 mingying   (501) staff       (20)     1605 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1395 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     3813 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/async_connections.py
+-rw-r--r--   0 mingying   (501) staff       (20)      308 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/async_connections.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    11045 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/base.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3514 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/base.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4419 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/connections.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1154 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/connections.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    10568 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/http_async.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1267 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/http_async.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     8719 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/http_requests.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1761 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/http_requests.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    10657 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/http_urllib3.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2191 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/http_urllib3.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2048 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/pooling.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1332 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection/pooling.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    11778 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection_pool.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3198 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/connection_pool.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5960 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/exceptions.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2275 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/exceptions.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.962596 retakesearch-py-2.2.5/opensearchpy/helpers/
+-rw-r--r--   0 mingying   (501) staff       (20)     1929 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2139 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    24406 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/actions.py
+-rw-r--r--   0 mingying   (501) staff       (20)     4186 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/actions.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     9849 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/aggs.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3487 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/aggs.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     8525 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/analysis.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2161 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/analysis.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1866 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/asyncsigner.py
+-rw-r--r--   0 mingying   (501) staff       (20)      595 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/asyncsigner.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    18613 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/document.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1347 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/document.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     1487 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/errors.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1378 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/errors.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    13797 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/faceted_search.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1374 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/faceted_search.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    14196 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/field.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2257 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/field.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     3857 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/function.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1459 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/function.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    22993 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/index.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1127 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/index.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     7960 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/mapping.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1155 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/mapping.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    12671 2023-08-07 20:06:34.000000 retakesearch-py-2.2.5/opensearchpy/helpers/query.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2952 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/query.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.963500 retakesearch-py-2.2.5/opensearchpy/helpers/response/
+-rw-r--r--   0 mingying   (501) staff       (20)     4409 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/response/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1205 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/response/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2946 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/response/aggs.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1315 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/response/aggs.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2161 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/response/hit.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1124 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/response/hit.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    27545 2023-08-07 20:54:12.000000 retakesearch-py-2.2.5/opensearchpy/helpers/search.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1313 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/search.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2900 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/signer.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3459 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/test.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1579 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/test.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     5344 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/update_by_query.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1132 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/update_by_query.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    19065 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/utils.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1238 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/utils.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     2868 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/wrappers.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1125 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/helpers/wrappers.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.964819 retakesearch-py-2.2.5/opensearchpy/plugins/
+-rw-r--r--   0 mingying   (501) staff       (20)      281 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/plugins/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)      279 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/plugins/__init__.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     6391 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/plugins/alerting.py
+-rw-r--r--   0 mingying   (501) staff       (20)     2396 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/plugins/alerting.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)     4863 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/plugins/index_management.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1988 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/plugins/index_management.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    21208 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/plugins/security.py
+-rw-r--r--   0 mingying   (501) staff       (20)     7652 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/plugins/security.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/py.typed
+-rw-r--r--   0 mingying   (501) staff       (20)     6226 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/serializer.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1876 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/serializer.pyi
+-rw-r--r--   0 mingying   (501) staff       (20)    18470 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/transport.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3507 2023-07-23 18:55:25.000000 retakesearch-py-2.2.5/opensearchpy/transport.pyi
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-08-07 22:45:26.965737 retakesearch-py-2.2.5/retakesearch_py.egg-info/
+-rw-r--r--   0 mingying   (501) staff       (20)     5636 2023-08-07 22:45:26.000000 retakesearch-py-2.2.5/retakesearch_py.egg-info/PKG-INFO
+-rw-r--r--   0 mingying   (501) staff       (20)     6173 2023-08-07 22:45:26.000000 retakesearch-py-2.2.5/retakesearch_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mingying   (501) staff       (20)        1 2023-08-07 22:45:26.000000 retakesearch-py-2.2.5/retakesearch_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-23 18:56:34.000000 retakesearch-py-2.2.5/retakesearch_py.egg-info/not-zip-safe
+-rw-r--r--   0 mingying   (501) staff       (20)      454 2023-08-07 22:45:26.000000 retakesearch-py-2.2.5/retakesearch_py.egg-info/requires.txt
+-rw-r--r--   0 mingying   (501) staff       (20)       13 2023-08-07 22:45:26.000000 retakesearch-py-2.2.5/retakesearch_py.egg-info/top_level.txt
+-rw-r--r--   0 mingying   (501) staff       (20)      280 2023-08-07 22:45:26.966181 retakesearch-py-2.2.5/setup.cfg
+-rw-r--r--   0 mingying   (501) staff       (20)     4775 2023-07-31 22:41:58.000000 retakesearch-py-2.2.5/setup.py
```

### Comparing `retakesearch-py-2.2.4/CONTRIBUTING.md` & `retakesearch-py-2.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/LICENSE.txt` & `retakesearch-py-2.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/PKG-INFO` & `retakesearch-py-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch-py
-Version: 2.2.4
+Version: 2.2.5
 Summary: Python client for OpenSearch
 Home-page: https://github.com/opensearch-project/opensearch-py
 Author: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Author-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 Maintainer: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Maintainer-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 License: Apache-2.0
```

### Comparing `retakesearch-py-2.2.4/README.md` & `retakesearch-py-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/__init__.py` & `retakesearch-py-2.2.5/opensearchpy/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/__init__.pyi` & `retakesearch-py-2.2.5/opensearchpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/__init__.py` & `retakesearch-py-2.2.5/opensearchpy/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/_extra_imports.py` & `retakesearch-py-2.2.5/opensearchpy/_async/_extra_imports.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/__init__.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/__init__.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/cat.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/cat.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/cat.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/cat.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/cluster.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/cluster.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/cluster.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/cluster.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/dangling_indices.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/dangling_indices.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/dangling_indices.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/dangling_indices.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/features.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/features.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/features.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/features.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/indices.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/indices.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/indices.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/indices.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/ingest.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/ingest.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/ingest.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/ingest.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/nodes.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/nodes.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/nodes.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/nodes.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/plugins.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/plugins.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/plugins.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/plugins.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/remote.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/remote.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/remote.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/remote.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/snapshot.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/snapshot.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/snapshot.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/snapshot.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/tasks.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/tasks.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/tasks.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/tasks.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/utils.py` & `retakesearch-py-2.2.5/opensearchpy/_async/client/utils.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/client/utils.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/client/utils.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/compat.py` & `retakesearch-py-2.2.5/opensearchpy/_async/compat.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/compat.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/compat.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/helpers/actions.py` & `retakesearch-py-2.2.5/opensearchpy/_async/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/helpers/actions.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/helpers/actions.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/helpers/document.py` & `retakesearch-py-2.2.5/opensearchpy/_async/helpers/document.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/helpers/faceted_search.py` & `retakesearch-py-2.2.5/opensearchpy/_async/helpers/faceted_search.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/helpers/index.py` & `retakesearch-py-2.2.5/opensearchpy/_async/helpers/index.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/helpers/mapping.py` & `retakesearch-py-2.2.5/opensearchpy/_async/helpers/mapping.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/helpers/search.py` & `retakesearch-py-2.2.5/opensearchpy/_async/helpers/search.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/helpers/test.py` & `retakesearch-py-2.2.5/opensearchpy/_async/helpers/test.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/helpers/test.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/helpers/test.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/helpers/update_by_query.py` & `retakesearch-py-2.2.5/opensearchpy/_async/helpers/update_by_query.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/http_aiohttp.py` & `retakesearch-py-2.2.5/opensearchpy/_async/http_aiohttp.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/http_aiohttp.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/http_aiohttp.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/plugins/alerting.py` & `retakesearch-py-2.2.5/opensearchpy/_async/plugins/alerting.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/plugins/alerting.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/plugins/alerting.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/plugins/index_management.py` & `retakesearch-py-2.2.5/opensearchpy/_async/plugins/index_management.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/plugins/index_management.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/plugins/index_management.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/plugins/security.py` & `retakesearch-py-2.2.5/opensearchpy/_async/plugins/security.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/plugins/security.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/plugins/security.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/transport.py` & `retakesearch-py-2.2.5/opensearchpy/_async/transport.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_async/transport.pyi` & `retakesearch-py-2.2.5/opensearchpy/_async/transport.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/_version.py` & `retakesearch-py-2.2.5/opensearchpy/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-__versionstr__ = "2.2.4"
+__versionstr__ = "2.2.5"
```

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/__init__.py` & `retakesearch-py-2.2.5/opensearchpy/client/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/__init__.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/cat.py` & `retakesearch-py-2.2.5/opensearchpy/client/cat.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/cat.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/cat.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/cluster.py` & `retakesearch-py-2.2.5/opensearchpy/client/cluster.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/cluster.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/cluster.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/dangling_indices.py` & `retakesearch-py-2.2.5/opensearchpy/client/dangling_indices.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/dangling_indices.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/dangling_indices.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/features.py` & `retakesearch-py-2.2.5/opensearchpy/client/features.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/features.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/features.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/indices.py` & `retakesearch-py-2.2.5/opensearchpy/client/indices.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/indices.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/indices.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/ingest.py` & `retakesearch-py-2.2.5/opensearchpy/client/ingest.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/ingest.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/ingest.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/nodes.py` & `retakesearch-py-2.2.5/opensearchpy/client/nodes.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/nodes.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/nodes.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/plugins.py` & `retakesearch-py-2.2.5/opensearchpy/client/plugins.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/plugins.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/plugins.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/remote.py` & `retakesearch-py-2.2.5/opensearchpy/client/remote.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/remote.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/remote.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/snapshot.py` & `retakesearch-py-2.2.5/opensearchpy/client/snapshot.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/snapshot.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/snapshot.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/tasks.py` & `retakesearch-py-2.2.5/opensearchpy/client/tasks.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/tasks.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/tasks.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/utils.py` & `retakesearch-py-2.2.5/opensearchpy/client/utils.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/client/utils.pyi` & `retakesearch-py-2.2.5/opensearchpy/client/utils.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/compat.py` & `retakesearch-py-2.2.5/opensearchpy/compat.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/compat.pyi` & `retakesearch-py-2.2.5/opensearchpy/compat.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/__init__.py` & `retakesearch-py-2.2.5/opensearchpy/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/__init__.pyi` & `retakesearch-py-2.2.5/opensearchpy/connection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/async_connections.py` & `retakesearch-py-2.2.5/opensearchpy/connection/async_connections.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/base.py` & `retakesearch-py-2.2.5/opensearchpy/connection/base.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/base.pyi` & `retakesearch-py-2.2.5/opensearchpy/connection/base.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/connections.py` & `retakesearch-py-2.2.5/opensearchpy/connection/connections.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/connections.pyi` & `retakesearch-py-2.2.5/opensearchpy/connection/connections.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/http_async.py` & `retakesearch-py-2.2.5/opensearchpy/connection/http_async.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/http_async.pyi` & `retakesearch-py-2.2.5/opensearchpy/connection/http_async.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/http_requests.py` & `retakesearch-py-2.2.5/opensearchpy/connection/http_requests.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/http_requests.pyi` & `retakesearch-py-2.2.5/opensearchpy/connection/http_requests.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/http_urllib3.py` & `retakesearch-py-2.2.5/opensearchpy/connection/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/http_urllib3.pyi` & `retakesearch-py-2.2.5/opensearchpy/connection/http_urllib3.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/pooling.py` & `retakesearch-py-2.2.5/opensearchpy/connection/pooling.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection/pooling.pyi` & `retakesearch-py-2.2.5/opensearchpy/connection/pooling.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection_pool.py` & `retakesearch-py-2.2.5/opensearchpy/connection_pool.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/connection_pool.pyi` & `retakesearch-py-2.2.5/opensearchpy/connection_pool.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/exceptions.py` & `retakesearch-py-2.2.5/opensearchpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/exceptions.pyi` & `retakesearch-py-2.2.5/opensearchpy/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/__init__.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/__init__.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/actions.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/actions.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/actions.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/aggs.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/aggs.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/aggs.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/aggs.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/analysis.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/analysis.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/analysis.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/analysis.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/asyncsigner.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/asyncsigner.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/asyncsigner.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/asyncsigner.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/document.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/document.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/document.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/document.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/errors.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/errors.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/errors.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/faceted_search.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/faceted_search.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/faceted_search.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/faceted_search.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/field.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/field.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/field.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/field.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/function.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/function.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/function.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/function.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/index.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/index.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/index.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/index.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/mapping.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/mapping.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/mapping.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/mapping.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/query.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/query.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/query.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/query.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/response/__init__.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/response/__init__.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/response/__init__.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/response/__init__.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/response/aggs.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/response/aggs.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/response/aggs.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/response/aggs.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/response/hit.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/response/hit.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/response/hit.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/response/hit.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/search.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/search.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/search.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/search.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/signer.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/signer.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/test.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/test.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/test.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/test.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/update_by_query.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/update_by_query.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/update_by_query.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/update_by_query.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/utils.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/utils.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/utils.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/wrappers.py` & `retakesearch-py-2.2.5/opensearchpy/helpers/wrappers.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/helpers/wrappers.pyi` & `retakesearch-py-2.2.5/opensearchpy/helpers/wrappers.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/plugins/alerting.py` & `retakesearch-py-2.2.5/opensearchpy/plugins/alerting.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/plugins/alerting.pyi` & `retakesearch-py-2.2.5/opensearchpy/plugins/alerting.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/plugins/index_management.py` & `retakesearch-py-2.2.5/opensearchpy/plugins/index_management.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/plugins/index_management.pyi` & `retakesearch-py-2.2.5/opensearchpy/plugins/index_management.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/plugins/security.py` & `retakesearch-py-2.2.5/opensearchpy/plugins/security.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/plugins/security.pyi` & `retakesearch-py-2.2.5/opensearchpy/plugins/security.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/serializer.py` & `retakesearch-py-2.2.5/opensearchpy/serializer.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/serializer.pyi` & `retakesearch-py-2.2.5/opensearchpy/serializer.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/transport.py` & `retakesearch-py-2.2.5/opensearchpy/transport.py`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/opensearchpy/transport.pyi` & `retakesearch-py-2.2.5/opensearchpy/transport.pyi`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/retakesearch_py.egg-info/PKG-INFO` & `retakesearch-py-2.2.5/retakesearch_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch-py
-Version: 2.2.4
+Version: 2.2.5
 Summary: Python client for OpenSearch
 Home-page: https://github.com/opensearch-project/opensearch-py
 Author: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Author-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 Maintainer: Aleksei Atavin, Denis Zalevskiy, Rushi Agrawal, Shephali Mittal
 Maintainer-email: axeo@aiven.io, dez@aiven.io, rushi.agr@gmail.com, shephalm@amazon.com
 License: Apache-2.0
```

### Comparing `retakesearch-py-2.2.4/retakesearch_py.egg-info/SOURCES.txt` & `retakesearch-py-2.2.5/retakesearch_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `retakesearch-py-2.2.4/setup.py` & `retakesearch-py-2.2.5/setup.py`

 * *Files identical despite different names*

