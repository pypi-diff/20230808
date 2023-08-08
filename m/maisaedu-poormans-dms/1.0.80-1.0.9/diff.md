# Comparing `tmp/maisaedu-poormans-dms-1.0.80.tar.gz` & `tmp/maisaedu-poormans-dms-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maisaedu-poormans-dms-1.0.80.tar", last modified: Tue Aug  8 20:47:29 2023, max compression
+gzip compressed data, was "maisaedu-poormans-dms-1.0.9.tar", last modified: Wed Nov 16 19:30:53 2022, max compression
```

## Comparing `maisaedu-poormans-dms-1.0.80.tar` & `maisaedu-poormans-dms-1.0.9.tar`

### file list

```diff
@@ -1,53 +1,30 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:29.703807 maisaedu-poormans-dms-1.0.80/
--rw-r--r--   0 vsts      (1001) docker     (123)     1076 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      289 2023-08-08 20:47:29.703807 maisaedu-poormans-dms-1.0.80/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:29.699807 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/
--rw-r--r--   0 vsts      (1001) docker     (123)    16086 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:29.699807 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:29.703807 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/Contracts/
--rw-r--r--   0 vsts      (1001) docker     (123)      510 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      395 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowReaderInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowWriterInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      189 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorTableInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/Contracts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2095 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/Migrator.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:29.703807 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/MigratorRow/
--rw-r--r--   0 vsts      (1001) docker     (123)     4663 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2998 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5047 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/MigratorRow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5178 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/MigratorTable.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:29.703807 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/
--rw-r--r--   0 vsts      (1001) docker     (123)     1881 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Connector.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:29.703807 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Contracts/
--rw-r--r--   0 vsts      (1001) docker     (123)      256 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Contracts/WriterInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Contracts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3831 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/MigratorRedshift.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:29.703807 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Models/
--rw-r--r--   0 vsts      (1001) docker     (123)      605 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Models/ExtractionOperation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1395 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Models/Struct.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6122 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Reader.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:29.703807 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Services/
--rw-r--r--   0 vsts      (1001) docker     (123)     3555 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Services/AdapterSourceTarget.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2821 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Services/ExtractionOperation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Services/Struct.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Services/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1266 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Types.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:29.703807 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Writer/
--rw-r--r--   0 vsts      (1001) docker     (123)     3191 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Writer/GenericWriter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5361 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Writer/WriterCDC.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1425 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Writer/WriterNonCDC.py
--rw-r--r--   0 vsts      (1001) docker     (123)      339 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/Writer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/redshift_migration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14790 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/sql_server_migration.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:29.699807 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      289 2023-08-08 20:47:29.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2301 2023-08-08 20:47:29.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-08 20:47:29.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      107 2023-08-08 20:47:29.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-08-08 20:47:29.000000 maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-08 20:47:29.703807 maisaedu-poormans-dms-1.0.80/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      644 2023-08-08 20:47:08.000000 maisaedu-poormans-dms-1.0.80/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.922747 maisaedu-poormans-dms-1.0.9/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1076 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2022-11-16 19:30:53.918747 maisaedu-poormans-dms-1.0.9/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.914747 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/
+-rw-r--r--   0 vsts      (1001) docker     (122)    16071 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.918747 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.918747 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/
+-rw-r--r--   0 vsts      (1001) docker     (122)      510 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      509 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowReaderInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      337 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowWriterInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      189 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorTableInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2095 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Migrator.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.918747 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4611 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3302 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4976 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4928 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorTable.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11139 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/sql_server_migration.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.914747 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2022-11-16 19:30:53.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1192 2022-11-16 19:30:53.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-11-16 19:30:53.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       75 2022-11-16 19:30:53.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       22 2022-11-16 19:30:53.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2022-11-16 19:30:53.922747 maisaedu-poormans-dms-1.0.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      578 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/setup.py
```

### Comparing `maisaedu-poormans-dms-1.0.80/LICENSE` & `maisaedu-poormans-dms-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/__init__.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from typing import List, Callable, Dict, Any, Iterable, Iterator, Optional, Union
 from enum import Enum
 
 from maisaedu_poormans_dms.sql_server_migration import (
     build_create_query,
     get_table_info_query,
     extract_load_data,
-    execute_sp
 )
 
 
 async def execute_once(pool: Pool, query: Union[str, bytes], args=()):
     """Executes a parametrized query in a pool once and streams the rows."""
     async with pool.acquire() as connection:
         async with connection.cursor() as cursor:
```

### Comparing `maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/Migrator.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Migrator.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from maisaedu_utilities_prefect.utils import build_prefect_logger
-
+import prefect
 from .Reader import MigratorReader
 from .Writer import MigratorWriter
 from ..Contracts.MigratorRowInterface import MigratorRowInterface
 from dataclasses import dataclass
 
 
 @dataclass
@@ -62,52 +61,52 @@
             self.copy_config,
             self.ignore_columns,
         )
 
     def __migrate_without_incremental_column(self):
         default_commit = False
 
-        build_prefect_logger().info(f"Truncating {self.target_table_name} table ...")
+        prefect.context.logger.info(f"Truncating {self.target_table_name} table ...")
         self.migrator_writer.truncate_target_table(default_commit)
-        build_prefect_logger().info(f"Table {self.target_table_name} truncated")
+        prefect.context.logger.info(f"Table {self.target_table_name} truncated")
 
-        build_prefect_logger().info(
+        prefect.context.logger.info(
             f"Getting data from {self.source_table_name} table in batches and inserting into {self.target_table_name} table ..."
         )
         columns_names = self.migrator_reader.get_columns_names(
             self.migrator_reader.get_source_query_without_incremental_column
         )
         batches = self.migrator_reader.get_source_data(
             self.migrator_reader.get_source_query_without_incremental_column, "full"
         )
         total_inserted = self.migrator_writer.insert_data_into_target_table(
             batches, columns_names, default_commit
         )
-        build_prefect_logger().info(
+        prefect.context.logger.info(
             f"Inserted {total_inserted} rows into {self.target_table_name} table"
         )
 
         self.target_conn.commit()
 
     def __migrate_with_incremental_column(self):
         default_commit = True
 
-        build_prefect_logger().info(
+        prefect.context.logger.info(
             f"Getting data from {self.source_table_name} table in batches and inserting into {self.target_table_name} table ..."
         )
         columns_names = self.migrator_reader.get_columns_names(
             self.migrator_reader.get_source_query_with_incremental_column
         )
         batches = self.migrator_reader.get_source_data(
             self.migrator_reader.get_source_query_with_incremental_column, "incremental"
         )
         total_inserted = self.migrator_writer.insert_data_into_target_table(
             batches, columns_names, default_commit
         )
-        build_prefect_logger().info(
+        prefect.context.logger.info(
             f"Inserted {total_inserted} rows into {self.target_table_name} table"
         )
 
     def migrate(
         self,
         source_table_name: str,
         target_table_name: str,
```

### Comparing `maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,21 +58,31 @@
         cursor.close()
         columns_names = [desc[0] for desc in cursor.description]
         return columns_names
 
     def get_source_data(self, function_get_source_query: object, type: str) -> list:
         source_query = function_get_source_query()
 
-        with self.source_conn.cursor(name="extract_cursor") as cursor:
-            cursor.itersize = self.read_batch_size
-            cursor.execute(source_query)
-
-            rows_to_return = []
-
-            for row in cursor:
-                rows_to_return.append(row)
-                if len(rows_to_return) >= self.read_batch_size:
-                    yield rows_to_return
-                    rows_to_return = []
+        cursor = self.source_conn.cursor()
 
-            if len(rows_to_return) >= 0:
-                yield rows_to_return
+        index = 0
+        offset = 0
+        batch_size = self.read_batch_size
+        cursor.execute(f"{source_query} offset {offset} limit {batch_size}")
+        rows = cursor.fetchall()
+
+        while len(rows) > 0:
+            yield rows
+
+            offset += len(rows)
+            index += 1
+            if (
+                type == "incremental" and index >= 20
+            ):  # this part reset query when it has more than 20 pages, because when incremental flow is used, it can be very slow
+                source_query = function_get_source_query()
+                index = 0
+                offset = 0
+
+            cursor.execute(f"{source_query} offset {offset} limit {batch_size}")
+            rows = cursor.fetchall()
+
+        cursor.close()
```

### Comparing `maisaedu-poormans-dms-1.0.80/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,14 @@
         self.target_table_name = target_table_name
         self.write_batch_size = write_batch_size
         self.on_conflict = on_conflict
         self.copy_config = copy_config
         self.ignore_columns = ignore_columns
 
     def __bind_on_conflict(self):
-        if self.on_conflict is True:
-            self.on_conflict = ''
         if self.on_conflict is None:
             return self.on_conflict
         if "[[all]]" in self.on_conflict.lower():
             result = select(
                 self.target_conn,
                 f"""
                 select STRING_AGG('"' || column_name || '"=excluded."' || column_name || '"', ', ')
```

### Comparing `maisaedu-poormans-dms-1.0.80/setup.py` & `maisaedu-poormans-dms-1.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="maisaedu-poormans-dms",
-    version="1.0.80",
+    version="1.0.9",
     description="A library for making database migration tasks, for +A Education",
     license="MIT License",
     author="A+ Educação",
     author_email="dataeng@maisaedu.com.br",
     packages=find_packages(),
     scripts=[],
     install_requires=[
         "pandas",
         "scipy",
         "numpy",
         "wheel",
         "psycopg2-binary",
         "aiopg",
         "aiochannel",
-        "pymssql==2.2.7",
+        "pymssql",
         "datetime",
-        "sqlalchemy",
-        "pyarrow",
-        "boto3",
     ],  # external packages as dependencies
 )
```

