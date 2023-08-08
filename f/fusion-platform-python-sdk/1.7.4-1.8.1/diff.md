# Comparing `tmp/fusion-platform-python-sdk-1.7.4.tar.gz` & `tmp/fusion-platform-python-sdk-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-platform-python-sdk-1.7.4.tar", last modified: Fri Jul  7 12:49:06 2023, max compression
+gzip compressed data, was "fusion-platform-python-sdk-1.8.1.tar", last modified: Tue Aug  8 09:04:02 2023, max compression
```

## Comparing `fusion-platform-python-sdk-1.7.4.tar` & `fusion-platform-python-sdk-1.8.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-07-07 12:49:06.870259 fusion-platform-python-sdk-1.7.4/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.7.4/LICENSE.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.7.4/MANIFEST.in
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-07-07 12:49:06.869967 fusion-platform-python-sdk-1.7.4/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4455 2023-06-26 08:49:45.000000 fusion-platform-python-sdk-1.7.4/README.md
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-07-07 12:49:06.856519 fusion-platform-python-sdk-1.7.4/fusion_platform/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     6865 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/__main__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/base.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/command.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-07-07 12:49:06.857895 fusion-platform-python-sdk-1.7.4/fusion_platform/common/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/common/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/common/raise_thread.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/common/utilities.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4579 2023-06-26 08:54:13.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/detailed_example.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/documentation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)  1593164 2023-06-07 06:22:45.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/fusion_platform_sdk.pdf
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4697 2023-07-06 06:17:51.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/glasgow.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)  3746742 2023-07-06 06:17:51.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/lake_district.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/localisations.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/localise.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-07-07 12:49:06.867282 fusion-platform-python-sdk-1.7.4/fusion_platform/models/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/credit.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/credit.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/data.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/data.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/data_file.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/data_file.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/fields.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    31868 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/model.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/organisation.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    14976 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/organisation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    50774 2023-07-07 12:47:31.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2602 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     8982 2023-07-06 09:45:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3359 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10513 2023-07-06 06:16:57.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution_log.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution_log.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/service.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     9735 2023-05-24 05:51:58.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/service.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/user.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/user.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1891 2023-06-26 08:54:13.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/quick_example.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/session.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     7576 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/translations.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-07-07 12:49:06.869448 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1773 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       77 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/requires.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2023-07-07 12:49:06.870365 fusion-platform-python-sdk-1.7.4/setup.cfg
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1551 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/setup.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-08-08 09:04:02.648111 fusion-platform-python-sdk-1.8.1/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.8.1/LICENSE.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.8.1/MANIFEST.in
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5126 2023-08-08 09:04:02.647830 fusion-platform-python-sdk-1.8.1/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4456 2023-08-08 06:50:33.000000 fusion-platform-python-sdk-1.8.1/README.md
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-08-08 09:04:02.630936 fusion-platform-python-sdk-1.8.1/fusion_platform/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     7151 2023-08-08 09:03:58.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/__main__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/base.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/command.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-08-08 09:04:02.633627 fusion-platform-python-sdk-1.8.1/fusion_platform/common/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/common/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/common/raise_thread.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/common/utilities.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4579 2023-08-08 07:27:21.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/detailed_example.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/documentation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  1652653 2023-08-08 06:58:34.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/fusion_platform_sdk.pdf
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4697 2023-07-06 06:17:51.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/glasgow.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  3746742 2023-07-06 06:17:51.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/lake_district.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/localisations.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/localise.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-08-08 09:04:02.645101 fusion-platform-python-sdk-1.8.1/fusion_platform/models/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2023-08-08 09:03:59.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/credit.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/credit.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2023-08-08 09:03:59.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/data.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/data.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2023-08-08 09:03:59.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/data_file.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/data_file.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/fields.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    31868 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/model.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2023-08-08 09:03:59.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/organisation.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    14976 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/organisation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2023-08-08 09:03:59.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/process.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    50774 2023-07-07 12:47:31.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/process.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2602 2023-08-08 09:03:59.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/process_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     8982 2023-07-06 09:45:04.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/process_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3359 2023-08-08 09:03:59.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/process_service_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10513 2023-07-06 06:16:57.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/process_service_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2023-08-08 09:03:59.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/process_service_execution_log.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/process_service_execution_log.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2023-08-08 09:03:59.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/service.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     9735 2023-05-24 05:51:58.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/service.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2023-08-08 09:03:59.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/user.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/models/user.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1891 2023-08-08 07:27:21.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/quick_example.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/session.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     7576 2023-08-08 09:03:59.000000 fusion-platform-python-sdk-1.8.1/fusion_platform/translations.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-08-08 09:04:02.647344 fusion-platform-python-sdk-1.8.1/fusion_platform_python_sdk.egg-info/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5126 2023-08-08 09:04:02.000000 fusion-platform-python-sdk-1.8.1/fusion_platform_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1773 2023-08-08 09:04:02.000000 fusion-platform-python-sdk-1.8.1/fusion_platform_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2023-08-08 09:04:02.000000 fusion-platform-python-sdk-1.8.1/fusion_platform_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       76 2023-08-08 09:04:02.000000 fusion-platform-python-sdk-1.8.1/fusion_platform_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2023-08-08 09:04:02.000000 fusion-platform-python-sdk-1.8.1/fusion_platform_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2023-08-08 09:04:02.000000 fusion-platform-python-sdk-1.8.1/fusion_platform_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2023-08-08 09:04:02.648207 fusion-platform-python-sdk-1.8.1/setup.cfg
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1552 2023-08-08 09:03:58.000000 fusion-platform-python-sdk-1.8.1/setup.py
```

### Comparing `fusion-platform-python-sdk-1.7.4/LICENSE.txt` & `fusion-platform-python-sdk-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/PKG-INFO` & `fusion-platform-python-sdk-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.7.4
+Version: 1.8.1
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Fusion Platform<sup>&reg;</sup> Python SDK
 
 This package contains the Python SDK used to interact with the Fusion Platform<sup>&reg;</sup>. The Fusion Platform<sup>&reg;</sup> provides enhanced remote
 monitoring services. By ingesting remotely sensed Earth Observation (EO) data, and data from other sources, the platform uses and fuses this data to execute
@@ -26,15 +25,15 @@
 files, create and execute processes, monitor their execution and then download the corresponding results. Additional functionality is available directly via the
 API, and this is defined within the corresponding OpenAPI 3.0 specification, which can be obtained via a support request.
 
 [&copy; Digital Content Analysis Technology Ltd](https://www.d-cat.co.uk)
 
 ## Installation
 
-The SDK has been built for Python 3, and is tested against Python 3.7, 3.8, 3.9 and 3.10. To install the SDK into a suitable Python environment containing `pip`,
+The SDK has been built for Python 3, and is tested against Python 3.8, 3.9, 3.10 and 3.11. To install the SDK into a suitable Python environment containing `pip`,
 execute the following:
 
 ```shell
 pip install fusion-platform-python-sdk
 ```
 
 This will install the SDK and all its dependencies.
@@ -117,8 +116,7 @@
 ## Support
 
 Support for the SDK can be obtained by contacting Digital Content Analysis Technology Ltd via [support@d-cat.co.uk](mailto:support@d-cat.co.uk).
 
 ## License
 
 See [LICENSE.txt](LICENSE.txt).
-
```

### Comparing `fusion-platform-python-sdk-1.7.4/README.md` & `fusion-platform-python-sdk-1.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 files, create and execute processes, monitor their execution and then download the corresponding results. Additional functionality is available directly via the
 API, and this is defined within the corresponding OpenAPI 3.0 specification, which can be obtained via a support request.
 
 [&copy; Digital Content Analysis Technology Ltd](https://www.d-cat.co.uk)
 
 ## Installation
 
-The SDK has been built for Python 3, and is tested against Python 3.7, 3.8, 3.9 and 3.10. To install the SDK into a suitable Python environment containing `pip`,
+The SDK has been built for Python 3, and is tested against Python 3.8, 3.9, 3.10 and 3.11. To install the SDK into a suitable Python environment containing `pip`,
 execute the following:
 
 ```shell
 pip install fusion-platform-python-sdk
 ```
 
 This will install the SDK and all its dependencies.
```

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/__init__.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 files, create and execute processes, monitor their execution and then download the corresponding results. Additional functionality is available directly via the
 API, and this is defined within the corresponding OpenAPI 3.0 specification, which can be obtained via a support request.
 
 &copy; [Digital Content Analysis Technology Ltd](https://www.d-cat.co.uk)
 """
 
 # Do not modify the following two lines as they are maintained by the version.sh script.
-__version__ = '1.7.4'
-__version_date__ = '2023-07-07T12:49:04Z'
+__version__ = '1.8.1'
+__version_date__ = '2023-08-08T09:03:58Z'
 
 # Exclude certain sub-modules from documentation.
 # @formatter:off
 __pdoc__ = {
     'base': False,
     'command': False,
     'common': False,
@@ -24,51 +24,56 @@
     'documentation': False,
     'localisations': False,
     'localise': False,
     'translations': False,
     'models.credit.CreditSchema.Meta': False,
     'models.credit.CreditSchema.opts': False,
     'models.credit.CreditSsdsSchema': False,
+    'models.credit.CreditMonthlySpendSchema': False,
     'models.data.DataSchema.Meta': False,
     'models.data.DataSchema.opts': False,
     'models.data_file.DataFileSchema.Meta': False,
     'models.data_file.DataFileSchema.opts': False,
     'models.data_file.DataFileSelectorSchema': False,
     'models.fields': False,
     'models.organisation.OrganisationSchema.Meta': False,
     'models.organisation.OrganisationSchema.opts': False,
     'models.organisation.OrganisationUserSchema': False,
     'models.process.ProcessSchema.Meta': False,
     'models.process.ProcessSchema.opts': False,
     'models.process.OptionDataTypeSchema': False,
     'models.process.ProcessChainOptionSchema': False,
     'models.process.ProcessChainSchema': False,
+    'models.process.ProcessExecutionStatusSchema': False,
+    'models.process.ProcessSelectorSchema': False,
     'models.process.ProcessInputSchema': False,
     'models.process.ProcessOptionSchema': False,
-    'models.process.ProcessSelectorSchema': False,
+    'models.process.ProcessDispatcherSchema': False,
     'models.process_execution.ProcessExecutionSchema.Meta': False,
     'models.process_execution.ProcessExecutionSchema.opts': False,
     'models.process_execution.ProcessExecutionChainOptionSchema': False,
     'models.process_execution.ProcessExecutionChainSchema': False,
     'models.process_execution.ProcessExecutionOptionSchema': False,
     'models.process_service_execution.ProcessServiceExecutionSchema.Meta': False,
     'models.process_service_execution.ProcessServiceExecutionSchema.opts': False,
-    'models.process_service_execution.ProcessServiceExecutionActionSchema': False,
     'models.process_service_execution.ProcessServiceExecutionActionValueSchema': False,
+    'models.process_service_execution.ProcessServiceExecutionActionSchema': False,
     'models.process_service_execution.ProcessServiceExecutionActionsSchema': False,
     'models.process_service_execution.ProcessServiceExecutionMetricSchema': False,
     'models.process_service_execution.ProcessServiceExecutionOptionSchema': False,
     'models.process_service_execution_log.ProcessServiceExecutionLogSchema.Meta': False,
     'models.process_service_execution_log.ProcessServiceExecutionLogSchema.opts': False,
     'models.service.ServiceSchema.Meta': False,
     'models.service.ServiceSchema.opts': False,
-    'models.service.ServiceActionSchema': False,
     'models.service.ServiceActionValueSchema': False,
+    'models.service.ServiceActionSchema': False,
     'models.service.ServiceDefinitionLinkageSchema': False,
     'models.service.ServiceDefinitionSchema': False,
+    'models.service.ServiceGroupAggregatorOptionSchema': False,
+    'models.service.ServiceGroupAggregatorSchema': False,
     'models.service.ServiceInputExpressionSchema': False,
     'models.service.ServiceOptionExpressionSchema': False,
     'models.service.ServiceValidationSchema': False,
     'models.user.UserSchema.Meta': False,
     'models.user.UserSchema.opts': False,
     'models.user.UserOrganisationSchema': False,
     'quick_example': False,
```

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/base.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/base.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/common/raise_thread.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/common/raise_thread.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/common/utilities.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/common/utilities.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/detailed_example.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/detailed_example.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/documentation.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/documentation.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/fusion_platform_sdk.pdf` & `fusion-platform-python-sdk-1.8.1/fusion_platform/fusion_platform_sdk.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 10% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,15 +1,15 @@
 Digital Content Analysis Technology Ltd
 
 Fusion Platform®
 
 Python SDK
 
-Version 1.7
-7th June 2023
+Version 1.8
+8th August 2023
 
 Digital Content Analysis Technology Ltd
 
 Table of Contents
 1
 
 Introduction ..................................................................................................... 4
@@ -232,14 +232,34 @@
 
 Version 1.7
 
 7th June 2023
 
 Issued for Fusion Platform® version 1.7.
 
+Draft
+
+th
+
+26 June 2023
+
+Extracted and tidied examples.
+
+Draft
+
+7th July 2023
+
+Added AWS S3 dispatcher example.
+
+Version 1.8
+
+8th August 2023
+
+Issued for Fusion Platform® version 1.8.
+
 This document has been prepared by Digital Content Analysis Technology Ltd, who can be
 contacted at support@d-cat.co.uk
 Digital Content Analysis Technology Ltd, Registered in Scotland, SC499652.
 This document is copyright and is issued on the strict understanding that it is not to be
 reproduced, copied, or disclosed to a third party, in whole or in part, without the consent of
 Digital Content Analysis Technology Ltd.
 © 2023 Digital Content Analysis Technology Ltd
@@ -399,15 +419,15 @@
 9. Delete the region of interest file
 When a region of interest file is no longer required, and it is not used by any process, then it
 can be explicitly deleted by the user (and therefore stop any further storage charges being
 incurred for it).
 2.3
 
 Installation
-The SDK has been built for Python 3, and is tested against Python 3.7, 3.8, 3.9 and 3.10. To
+The SDK has been built for Python 3, and is tested against Python 3.8, 3.9, 3.10 and 3.11. To
 install the SDK into a suitable Python environment containing “pip”, execute the following:
 Command
 pip install fusion-platform-python-sdk
 
 This will install the SDK and all its dependencies.
 To update an existing installation to the latest version, execute the following:
 Command
@@ -1032,18 +1052,55 @@
 Digital Content Analysis Technology Ltd
 
 To remove a dispatcher, use the following:
 Python
 # Remove the first dispatcher from the list of those added.
 process.remove_dispatcher(number=1)
 
+As an example, the AWS S3 dispatcher can be used to automatically write the outputs from a
+process to any destination S3 bucket. The dispatcher must be configured with the name of the
+destination bucket via the ‘bucket’ option. Where credentials are required to write to the
+bucket, then these may be set via the ‘access_key_id’ and ‘secret_access_key’
+options, and the optional ‘session_token’.
+Important
+
+As an alternative to providing credentials to the AWS S3 dispatcher, a policy can be set
+on the destination bucket which will allow the dispatcher to automatically write to the
+bucket. This is:
+{
+"Version": "2012-10-17",
+"Statement": [
+{
+"Sid": "DelegateS3Access",
+"Effect": "Allow",
+"Principal": {
+"AWS": [
+"arn:aws:iam::542134873422:role/FargatePrivilegedTaskRole"
+]
+},
+"Action": "s3:PutObject",
+"Resource": [
+"arn:aws:s3:::<NAME-OF_BUCKET>",
+"arn:aws:s3:::<NAME-OF_BUCKET>/*"
+]
+}
+]
+}
+
+Where ‘<NAME-OF-BUCKET>’ should be replaced with the name of the bucket. Note
+that if an alternative ‘api_url’ is being used during login, then a different AWS
+account number will be required in this bucket policy.
 When the process has been correctly configured, it can be saved to the Fusion Platform®.
 During this creation, the process will be validated and its corresponding price per execution
 calculated. If the process fails validation, then an exception will be thrown, and the process
 will not be saved.
+
+24
+
+Digital Content Analysis Technology Ltd
 Python
 # Attempt to create the process which will first validate it.
 # This will throw an exception if the validation fails.
 process.create()
 # Once created, the price will be available to review.
 print(process.price)
 Important
@@ -1068,18 +1125,14 @@
 then = datetime.now(timezone.utc) + timedelta(days=1)
 process_copy.update(
 run_type=fusion_platform.RUN_TYPE_RUN_SCHEDULE,
 repeat_count=1, repeat_start=then)
 # The copied process may then be created.
 process_copy.create()
 
-24
-
-Digital Content Analysis Technology Ltd
-
 When the process is no longer needed, it may be deleted:
 Python
 # Delete the process:
 process.delete()
 
 This will raise an exception in case of insufficient privileges, otherwise the process will be
 deleted. This will first stop any current executions and prevent any further executions taking
@@ -1345,18 +1398,16 @@
 The example uses a pre-defined region of interest of the Lake District in the UK, and then
 performs cloud classification over the region for a specific date using Sentinel-2. Since the
 region is relatively large, its execution is split. The example shows how to obtain aggregated
 statistics and how the split results can be combined into a single GeoTIFF, as well as how to
 work with the metadata generated for each file.
 Python
 from datetime import datetime, timezone
-import os
 import rasterio
 from rasterio.merge import merge
-from rasterio.plot import show
 import matplotlib.pyplot as pyplot
 import pandas
 import fusion_platform
 # Login with email address and password.
 user = fusion_platform.login(email='me@org.com',
 password='MyPassword123!')
 # Select the organisation which will own the file. This is
```

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/glasgow.geojson` & `fusion-platform-python-sdk-1.8.1/fusion_platform/glasgow.geojson`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/lake_district.geojson` & `fusion-platform-python-sdk-1.8.1/fusion_platform/lake_district.geojson`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/localisations.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/localisations.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/localise.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/localise.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/credit.md` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/credit.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/credit.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/credit.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/data.md` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/data.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/data.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/data.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/data_file.md` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/data_file.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/data_file.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/data_file.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/fields.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/fields.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/model.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/model.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/organisation.md` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/organisation.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/organisation.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/organisation.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process.md` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/process.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/process.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_execution.md` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/process_execution.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_execution.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/process_execution.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution.md` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/process_service_execution.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/process_service_execution.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution_log.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/process_service_execution_log.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/service.md` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/service.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/service.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/service.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/user.md` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/user.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/models/user.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/models/user.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/quick_example.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/quick_example.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/session.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/session.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform/translations.py` & `fusion-platform-python-sdk-1.8.1/fusion_platform/translations.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/PKG-INFO` & `fusion-platform-python-sdk-1.8.1/fusion_platform_python_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.7.4
+Version: 1.8.1
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Fusion Platform<sup>&reg;</sup> Python SDK
 
 This package contains the Python SDK used to interact with the Fusion Platform<sup>&reg;</sup>. The Fusion Platform<sup>&reg;</sup> provides enhanced remote
 monitoring services. By ingesting remotely sensed Earth Observation (EO) data, and data from other sources, the platform uses and fuses this data to execute
@@ -26,15 +25,15 @@
 files, create and execute processes, monitor their execution and then download the corresponding results. Additional functionality is available directly via the
 API, and this is defined within the corresponding OpenAPI 3.0 specification, which can be obtained via a support request.
 
 [&copy; Digital Content Analysis Technology Ltd](https://www.d-cat.co.uk)
 
 ## Installation
 
-The SDK has been built for Python 3, and is tested against Python 3.7, 3.8, 3.9 and 3.10. To install the SDK into a suitable Python environment containing `pip`,
+The SDK has been built for Python 3, and is tested against Python 3.8, 3.9, 3.10 and 3.11. To install the SDK into a suitable Python environment containing `pip`,
 execute the following:
 
 ```shell
 pip install fusion-platform-python-sdk
 ```
 
 This will install the SDK and all its dependencies.
@@ -117,8 +116,7 @@
 ## Support
 
 Support for the SDK can be obtained by contacting Digital Content Analysis Technology Ltd via [support@d-cat.co.uk](mailto:support@d-cat.co.uk).
 
 ## License
 
 See [LICENSE.txt](LICENSE.txt).
-
```

### Comparing `fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/SOURCES.txt` & `fusion-platform-python-sdk-1.8.1/fusion_platform_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.4/setup.py` & `fusion-platform-python-sdk-1.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 # Find the package root directory.
 PACKAGE_DIR = pathlib.Path(__file__).parent
 
 # Set up the package.
 # @formatter:off
 setup(
     name='fusion-platform-python-sdk',
-    version='1.7.4',
+    version='1.8.1',
     description='Python SDK used to interact with the Fusion Platform(r)',
     long_description=(PACKAGE_DIR / 'README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/d-cat-support/fusion-platform-python-sdk',
     author='Digital Content Analysis Technology Ltd',
     author_email='support@d-cat.co.uk',
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
     packages=find_packages(exclude='tests'),
     include_package_data=True,
     install_requires=[
         'marshmallow',
         'pyjwt',
         'python-dateutil',
```

