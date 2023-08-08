# Comparing `tmp/dbt-teradata-1.4.0.0.tar.gz` & `tmp/dbt-teradata-1.5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-teradata-1.4.0.0.tar", last modified: Thu Jul  6 07:17:36 2023, max compression
+gzip compressed data, was "dbt-teradata-1.5.0.0.tar", last modified: Tue Aug  8 10:22:41 2023, max compression
```

## Comparing `dbt-teradata-1.4.0.0.tar` & `dbt-teradata-1.5.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21442 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.442156 dbt-teradata-1.4.0.0/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.442156 dbt-teradata-1.4.0.0/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.446156 dbt-teradata-1.4.0.0/dbt/adapters/teradata/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 07:17:33.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/adapters/teradata/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.442156 dbt-teradata-1.4.0.0/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.446156 dbt-teradata-1.4.0.0/dbt/include/teradata/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.446156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/columns.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.442156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.446156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/seed/
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/test/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/test/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 07:16:41.000000 dbt-teradata-1.4.0.0/dbt/include/teradata/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-07-06 07:17:36.000000 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-06 07:17:36.000000 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:17:36.000000 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 07:17:36.000000 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 07:17:36.000000 dbt-teradata-1.4.0.0/dbt_teradata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 07:17:36.450156 dbt-teradata-1.4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-06 07:17:33.000000 dbt-teradata-1.4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.537583 dbt-teradata-1.5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22190 2023-08-08 10:22:41.525583 dbt-teradata-1.5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.521583 dbt-teradata-1.5.0.0/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.521583 dbt-teradata-1.5.0.0/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.521583 dbt-teradata-1.5.0.0/dbt/adapters/teradata/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/adapters/teradata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 10:22:38.000000 dbt-teradata-1.5.0.0/dbt/adapters/teradata/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/adapters/teradata/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/adapters/teradata/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/adapters/teradata/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/adapters/teradata/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.521583 dbt-teradata-1.5.0.0/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.521583 dbt-teradata-1.5.0.0/dbt/include/teradata/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.525583 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/columns.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.521583 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.525583 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.525583 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/seed/
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.525583 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.525583 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/test/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-08 10:21:47.000000 dbt-teradata-1.5.0.0/dbt/include/teradata/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:22:41.525583 dbt-teradata-1.5.0.0/dbt_teradata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22190 2023-08-08 10:22:41.000000 dbt-teradata-1.5.0.0/dbt_teradata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-08 10:22:41.000000 dbt-teradata-1.5.0.0/dbt_teradata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 10:22:41.000000 dbt-teradata-1.5.0.0/dbt_teradata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 10:22:41.000000 dbt-teradata-1.5.0.0/dbt_teradata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-08 10:22:41.000000 dbt-teradata-1.5.0.0/dbt_teradata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 10:22:41.537583 dbt-teradata-1.5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-08 10:22:38.000000 dbt-teradata-1.5.0.0/setup.py
```

### Comparing `dbt-teradata-1.4.0.0/LICENSE` & `dbt-teradata-1.5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/PKG-INFO` & `dbt-teradata-1.5.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-teradata
-Version: 1.4.0.0
+Version: 1.5.0.0
 Summary: The Teradata adapter plugin for dbt (data build tool)
 Home-page: https://github.com/Teradata/dbt-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-teradata
 
-This plugin ports [dbt](https://getdbt.com) functionality to Teradata Vantage.
+The dbt Teradata adapter lets you use [dbt](https://getdbt.com) with Teradata Vantage.
+
+**_NOTE:_** This adapter is maintained by Teradata. We are accelerating our release cadence. Starting October 1st, 2023, we will release `dbt-teradata` within 4 weeks of a minor release or within 8 weeks of a major release of `dbt-core`.
 
 ## Installation
 
 ```
 pip install dbt-teradata
 ```
 
@@ -66,14 +68,15 @@
 | 0.20.0.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
 | 0.21.1.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
 | 1.0.0.x           | ❌           | ✅          | ✅          | ✅          | ❌          | ❌
 |1.1.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
 |1.2.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
 |1.3.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
 |1.4.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ✅
+|1.5.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ✅
 
 
 ##  dbt dependent packages version compatibility
 | dbt-teradta |  dbt-core  | dbt-teradata-util |  dbt-util      |
 |-------------|------------|-------------------|----------------|
 | 1.2.x       | 1.2.x      | 0.1.0             | 0.9.x or below |
 
@@ -582,14 +585,17 @@
     post_hook=[
       "COLLECT STATISTICS ON  {{ this }} COLUMN (column_1,  column_2  ...);"
       ]
   )}}
   ```
   See [Collecting Statistics documentation](https://docs.teradata.com/r/76g1CuvvQlYBjb2WPIuk3g/RAyUdGfvREwbO9J0DMNpLw) for more information.
 
+## Support for model contracts
+Model constracts are not yet supported with dbt-teradata.
+
 ## Support for `dbt-utils` package
 `dbt-utils` package is supported through `teradata/teradata_utils` dbt package. The package provides a compatibility layer between `dbt_utils` and `dbt-teradata`. See [teradata_utils](https://hub.getdbt.com/teradata/teradata_utils/latest/) package for install instructions.
 
 ## Limitations
 
 ### Transaction mode
 Only ANSI transaction mode is supported.
```

### Comparing `dbt-teradata-1.4.0.0/README.md` & `dbt-teradata-1.5.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # dbt-teradata
 
-This plugin ports [dbt](https://getdbt.com) functionality to Teradata Vantage.
+The dbt Teradata adapter lets you use [dbt](https://getdbt.com) with Teradata Vantage.
+
+**_NOTE:_** This adapter is maintained by Teradata. We are accelerating our release cadence. Starting October 1st, 2023, we will release `dbt-teradata` within 4 weeks of a minor release or within 8 weeks of a major release of `dbt-core`.
 
 ## Installation
 
 ```
 pip install dbt-teradata
 ```
 
@@ -43,14 +45,15 @@
 | 0.20.0.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
 | 0.21.1.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
 | 1.0.0.x           | ❌           | ✅          | ✅          | ✅          | ❌          | ❌
 |1.1.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
 |1.2.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
 |1.3.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
 |1.4.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ✅
+|1.5.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ✅
 
 
 ##  dbt dependent packages version compatibility
 | dbt-teradta |  dbt-core  | dbt-teradata-util |  dbt-util      |
 |-------------|------------|-------------------|----------------|
 | 1.2.x       | 1.2.x      | 0.1.0             | 0.9.x or below |
 
@@ -559,14 +562,17 @@
     post_hook=[
       "COLLECT STATISTICS ON  {{ this }} COLUMN (column_1,  column_2  ...);"
       ]
   )}}
   ```
   See [Collecting Statistics documentation](https://docs.teradata.com/r/76g1CuvvQlYBjb2WPIuk3g/RAyUdGfvREwbO9J0DMNpLw) for more information.
 
+## Support for model contracts
+Model constracts are not yet supported with dbt-teradata.
+
 ## Support for `dbt-utils` package
 `dbt-utils` package is supported through `teradata/teradata_utils` dbt package. The package provides a compatibility layer between `dbt_utils` and `dbt-teradata`. See [teradata_utils](https://hub.getdbt.com/teradata/teradata_utils/latest/) package for install instructions.
 
 ## Limitations
 
 ### Transaction mode
 Only ANSI transaction mode is supported.
```

### Comparing `dbt-teradata-1.4.0.0/dbt/adapters/teradata/__init__.py` & `dbt-teradata-1.5.0.0/dbt/adapters/teradata/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/adapters/teradata/column.py` & `dbt-teradata-1.5.0.0/dbt/adapters/teradata/column.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/adapters/teradata/connections.py` & `dbt-teradata-1.5.0.0/dbt/adapters/teradata/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/adapters/teradata/impl.py` & `dbt-teradata-1.5.0.0/dbt/adapters/teradata/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/adapters/teradata/relation.py` & `dbt-teradata-1.5.0.0/dbt/adapters/teradata/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/adapters.sql` & `dbt-teradata-1.5.0.0/dbt/include/teradata/macros/adapters.sql`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 
 {% macro teradata__create_table_as(temporary, relation, sql) -%}
   {%- set sql_header = config.get('sql_header', none) -%}
   {%- set table_kind = config.get('table_kind', default='') -%}
   {%- set table_option = config.get('table_option', default='') -%}
   {%- set with_statistics = config.get('with_statistics', default=False)| as_bool -%}
   {%- set index = config.get('index', default='') -%}
+  {% set contract_config = config.get('contract') %}
+  {% if contract_config and contract_config.enforced %}
+    {{ exceptions.raise_compiler_error('Model contracts are not currently supported.') }}
+  {% endif %}
 
   {{ sql_header if sql_header is not none }}
   CREATE {{ table_kind }} TABLE
   {{ relation.include(database=False) }}
   {% if table_option |length -%}
   , {{ table_option }}
   {%- endif -%}
@@ -51,14 +55,18 @@
   {{ index }}
   {%- endif -%};
 
 {% endmacro %}
 
 {% macro teradata__create_view_as(relation, sql) -%}
   {%- set sql_header = config.get('sql_header', none) -%}
+  {% set contract_config = config.get('contract') %}
+  {% if contract_config and contract_config.enforced %}
+    {{ exceptions.raise_compiler_error('Model contracts are not currently supported.') }}
+  {% endif %}
 
   {{ sql_header if sql_header is not none }}
   REPLACE VIEW {{ relation.include(database=False) }} AS
     {{ sql }}
 
 {% endmacro %}
```

### Comparing `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/apply_grants.sql` & `dbt-teradata-1.5.0.0/dbt/include/teradata/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/catalog.sql` & `dbt-teradata-1.5.0.0/dbt/include/teradata/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/columns.sql` & `dbt-teradata-1.5.0.0/dbt/include/teradata/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql` & `dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql` & `dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/incremental/strategies.sql` & `dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/seed/seed.sql` & `dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql` & `dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt/include/teradata/macros/materializations/test/test.sql` & `dbt-teradata-1.5.0.0/dbt/include/teradata/macros/materializations/test/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/dbt_teradata.egg-info/PKG-INFO` & `dbt-teradata-1.5.0.0/dbt_teradata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-teradata
-Version: 1.4.0.0
+Version: 1.5.0.0
 Summary: The Teradata adapter plugin for dbt (data build tool)
 Home-page: https://github.com/Teradata/dbt-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dbt-teradata
 
-This plugin ports [dbt](https://getdbt.com) functionality to Teradata Vantage.
+The dbt Teradata adapter lets you use [dbt](https://getdbt.com) with Teradata Vantage.
+
+**_NOTE:_** This adapter is maintained by Teradata. We are accelerating our release cadence. Starting October 1st, 2023, we will release `dbt-teradata` within 4 weeks of a minor release or within 8 weeks of a major release of `dbt-core`.
 
 ## Installation
 
 ```
 pip install dbt-teradata
 ```
 
@@ -66,14 +68,15 @@
 | 0.20.0.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
 | 0.21.1.x           | ✅          | ✅          | ✅          | ✅          | ❌          | ❌
 | 1.0.0.x           | ❌           | ✅          | ✅          | ✅          | ❌          | ❌
 |1.1.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
 |1.2.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
 |1.3.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ❌
 |1.4.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ✅
+|1.5.x.x            | ❌           | ✅          | ✅          | ✅          | ✅          | ✅
 
 
 ##  dbt dependent packages version compatibility
 | dbt-teradta |  dbt-core  | dbt-teradata-util |  dbt-util      |
 |-------------|------------|-------------------|----------------|
 | 1.2.x       | 1.2.x      | 0.1.0             | 0.9.x or below |
 
@@ -582,14 +585,17 @@
     post_hook=[
       "COLLECT STATISTICS ON  {{ this }} COLUMN (column_1,  column_2  ...);"
       ]
   )}}
   ```
   See [Collecting Statistics documentation](https://docs.teradata.com/r/76g1CuvvQlYBjb2WPIuk3g/RAyUdGfvREwbO9J0DMNpLw) for more information.
 
+## Support for model contracts
+Model constracts are not yet supported with dbt-teradata.
+
 ## Support for `dbt-utils` package
 `dbt-utils` package is supported through `teradata/teradata_utils` dbt package. The package provides a compatibility layer between `dbt_utils` and `dbt-teradata`. See [teradata_utils](https://hub.getdbt.com/teradata/teradata_utils/latest/) package for install instructions.
 
 ## Limitations
 
 ### Transaction mode
 Only ANSI transaction mode is supported.
```

### Comparing `dbt-teradata-1.4.0.0/dbt_teradata.egg-info/SOURCES.txt` & `dbt-teradata-1.5.0.0/dbt_teradata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.4.0.0/setup.py` & `dbt-teradata-1.5.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 package_name = "dbt-teradata"
-package_version = "1.4.0.0"
+package_version = "1.5.0.0"
 description = """The Teradata adapter plugin for dbt (data build tool)"""
 
 
 setup(
     name=package_name,
     version=package_version,
 
@@ -41,15 +41,15 @@
             'macros/*.sql',
             'macros/materializations/**/*.sql',
             'dbt_project.yml',
             'sample_profiles.yml',
         ],
     },
     install_requires=[
-        "dbt-core==1.4.6",
+        "dbt-core==1.5.4",
         "teradatasql>=16.20.0.0",
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
 
         'License :: OSI Approved :: Apache Software License',
```

