# Comparing `tmp/types-aiobotocore-dms-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-dms-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dms-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-dms-2.5.4.tar", last modified: Tue Aug  8 01:23:36 2023, max compression
```

## Comparing `types-aiobotocore-dms-2.5.2.post3.tar` & `types-aiobotocore-dms-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.727647 types-aiobotocore-dms-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:21:35.000000 types-aiobotocore-dms-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17015 2023-08-04 12:37:36.719647 types-aiobotocore-dms-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-08-04 12:21:35.000000 types-aiobotocore-dms-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:36.727647 types-aiobotocore-dms-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-04 12:21:34.000000 types-aiobotocore-dms-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.715647 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-08-04 12:21:35.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-08-04 12:21:35.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-04 12:21:35.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69101 2023-08-04 12:21:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    69002 2023-08-04 12:21:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-08-04 12:21:37.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-08-04 12:21:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17787 2023-08-04 12:21:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-08-04 12:21:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:21:35.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    92903 2023-08-04 12:21:38.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    92852 2023-08-04 12:21:37.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:21:35.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-04 12:21:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-08-04 12:21:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:36.719647 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17015 2023-08-04 12:37:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:37:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:36.000000 types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:36.550686 types-aiobotocore-dms-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:09:10.000000 types-aiobotocore-dms-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-08-08 01:23:36.550686 types-aiobotocore-dms-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-08-08 01:09:10.000000 types-aiobotocore-dms-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:36.550686 types-aiobotocore-dms-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-08 01:09:09.000000 types-aiobotocore-dms-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:36.550686 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-08-08 01:09:10.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-08-08 01:09:10.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-08 01:09:10.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77084 2023-08-08 01:09:10.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76975 2023-08-08 01:09:10.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-08-08 01:09:11.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15236 2023-08-08 01:09:11.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17787 2023-08-08 01:09:11.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-08-08 01:09:11.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:09:10.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   105263 2023-08-08 01:09:13.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105200 2023-08-08 01:09:12.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:09:10.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-08 01:09:11.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-08-08 01:09:11.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:36.550686 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-08-08 01:23:36.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 01:23:36.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:36.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:36.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:36.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:36.000000 types-aiobotocore-dms-2.5.4/types_aiobotocore_dms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/LICENSE` & `types-aiobotocore-dms-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post3/PKG-INFO` & `types-aiobotocore-dms-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dms
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dms)](https://pepy.tech/project/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DatabaseMigrationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[aiobotocore.DatabaseMigrationService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/README.md` & `types-aiobotocore-dms-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dms)](https://pepy.tech/project/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DatabaseMigrationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[aiobotocore.DatabaseMigrationService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/setup.py` & `types-aiobotocore-dms-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dms",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_dms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.DatabaseMigrationService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/__init__.py` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/__init__.pyi` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/__main__.py` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DatabaseMigrationService 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.DatabaseMigrationService 2.5.4\nVersion:        "
+        " 2.5.4\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post3")
+    print("2.5.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/client.py` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,51 +43,58 @@
     DescribeTableStatisticsPaginator,
 )
 from .type_defs import (
     ApplyPendingMaintenanceActionResponseTypeDef,
     BatchStartRecommendationsResponseTypeDef,
     BlobTypeDef,
     CancelReplicationTaskAssessmentRunResponseTypeDef,
+    ComputeConfigTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     CreateFleetAdvisorCollectorResponseTypeDef,
+    CreateReplicationConfigResponseTypeDef,
     CreateReplicationInstanceResponseTypeDef,
     CreateReplicationSubnetGroupResponseTypeDef,
     CreateReplicationTaskResponseTypeDef,
     DeleteCertificateResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     DeleteEndpointResponseTypeDef,
     DeleteEventSubscriptionResponseTypeDef,
     DeleteFleetAdvisorDatabasesResponseTypeDef,
+    DeleteReplicationConfigResponseTypeDef,
     DeleteReplicationInstanceResponseTypeDef,
     DeleteReplicationTaskAssessmentRunResponseTypeDef,
     DeleteReplicationTaskResponseTypeDef,
     DescribeAccountAttributesResponseTypeDef,
     DescribeApplicableIndividualAssessmentsResponseTypeDef,
     DescribeCertificatesResponseTypeDef,
     DescribeConnectionsResponseTypeDef,
     DescribeEndpointSettingsResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeEndpointTypesResponseTypeDef,
+    DescribeEngineVersionsResponseTypeDef,
     DescribeEventCategoriesResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeEventSubscriptionsResponseTypeDef,
     DescribeFleetAdvisorCollectorsResponseTypeDef,
     DescribeFleetAdvisorDatabasesResponseTypeDef,
     DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
     DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
     DescribeFleetAdvisorSchemasResponseTypeDef,
     DescribeOrderableReplicationInstancesResponseTypeDef,
     DescribePendingMaintenanceActionsResponseTypeDef,
     DescribeRecommendationLimitationsResponseTypeDef,
     DescribeRecommendationsResponseTypeDef,
     DescribeRefreshSchemasStatusResponseTypeDef,
+    DescribeReplicationConfigsResponseTypeDef,
     DescribeReplicationInstancesResponseTypeDef,
     DescribeReplicationInstanceTaskLogsResponseTypeDef,
+    DescribeReplicationsResponseTypeDef,
     DescribeReplicationSubnetGroupsResponseTypeDef,
+    DescribeReplicationTableStatisticsResponseTypeDef,
     DescribeReplicationTaskAssessmentResultsResponseTypeDef,
     DescribeReplicationTaskAssessmentRunsResponseTypeDef,
     DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
     DescribeReplicationTasksResponseTypeDef,
     DescribeSchemasResponseTypeDef,
     DescribeTableStatisticsResponseTypeDef,
     DmsTransferSettingsTypeDef,
@@ -101,41 +108,46 @@
     ImportCertificateResponseTypeDef,
     KafkaSettingsTypeDef,
     KinesisSettingsTypeDef,
     ListTagsForResourceResponseTypeDef,
     MicrosoftSQLServerSettingsTypeDef,
     ModifyEndpointResponseTypeDef,
     ModifyEventSubscriptionResponseTypeDef,
+    ModifyReplicationConfigResponseTypeDef,
     ModifyReplicationInstanceResponseTypeDef,
     ModifyReplicationSubnetGroupResponseTypeDef,
     ModifyReplicationTaskResponseTypeDef,
     MongoDbSettingsTypeDef,
     MoveReplicationTaskResponseTypeDef,
     MySQLSettingsTypeDef,
     NeptuneSettingsTypeDef,
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
     RebootReplicationInstanceResponseTypeDef,
     RecommendationSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     RefreshSchemasResponseTypeDef,
+    ReloadReplicationTablesResponseTypeDef,
     ReloadTablesResponseTypeDef,
     RunFleetAdvisorLsaAnalysisResponseTypeDef,
     S3SettingsTypeDef,
     StartRecommendationsRequestEntryTypeDef,
+    StartReplicationResponseTypeDef,
     StartReplicationTaskAssessmentResponseTypeDef,
     StartReplicationTaskAssessmentRunResponseTypeDef,
     StartReplicationTaskResponseTypeDef,
+    StopReplicationResponseTypeDef,
     StopReplicationTaskResponseTypeDef,
     SybaseSettingsTypeDef,
     TableToReloadTypeDef,
     TagTypeDef,
     TestConnectionResponseTypeDef,
     TimestampTypeDef,
+    TimestreamSettingsTypeDef,
     UpdateSubscriptionsToEventBridgeResponseTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     ReplicationInstanceAvailableWaiter,
     ReplicationInstanceDeletedWaiter,
     ReplicationTaskDeletedWaiter,
@@ -299,15 +311,16 @@
         OracleSettings: OracleSettingsTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
-        GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
+        GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
+        TimestreamSettings: TimestreamSettingsTypeDef = ...
     ) -> CreateEndpointResponseTypeDef:
         """
         Creates an endpoint using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_endpoint)
         """
@@ -341,14 +354,36 @@
         """
         Creates a Fleet Advisor collector using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_fleet_advisor_collector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_fleet_advisor_collector)
         """
 
+    async def create_replication_config(
+        self,
+        *,
+        ReplicationConfigIdentifier: str,
+        SourceEndpointArn: str,
+        TargetEndpointArn: str,
+        ComputeConfig: ComputeConfigTypeDef,
+        ReplicationType: MigrationTypeValueType,
+        TableMappings: str,
+        ReplicationSettings: str = ...,
+        SupplementalSettings: str = ...,
+        ResourceIdentifier: str = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> CreateReplicationConfigResponseTypeDef:
+        """
+        Creates a configuration that you can later provide to configure and start an DMS
+        Serverless replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_config)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_replication_config)
+        """
+
     async def create_replication_instance(
         self,
         *,
         ReplicationInstanceIdentifier: str,
         ReplicationInstanceClass: str,
         AllocatedStorage: int = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
@@ -463,14 +498,24 @@
         """
         Deletes the specified Fleet Advisor collector databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_fleet_advisor_databases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#delete_fleet_advisor_databases)
         """
 
+    async def delete_replication_config(
+        self, *, ReplicationConfigArn: str
+    ) -> DeleteReplicationConfigResponseTypeDef:
+        """
+        Deletes an DMS Serverless replication configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_config)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#delete_replication_config)
+        """
+
     async def delete_replication_instance(
         self, *, ReplicationInstanceArn: str
     ) -> DeleteReplicationInstanceResponseTypeDef:
         """
         Deletes the specified replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_instance)
@@ -582,14 +627,24 @@
         """
         Returns information about the endpoints for your account in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_endpoints)
         """
 
+    async def describe_engine_versions(
+        self, *, MaxRecords: int = ..., Marker: str = ...
+    ) -> DescribeEngineVersionsResponseTypeDef:
+        """
+        Returns information about the replication instance versions used in the project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_engine_versions)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_engine_versions)
+        """
+
     async def describe_event_categories(
         self, *, SourceType: str = ..., Filters: Sequence[FilterTypeDef] = ...
     ) -> DescribeEventCategoriesResponseTypeDef:
         """
         Lists categories for all event source types, or, if specified, for a specified
         source type.
 
@@ -739,14 +794,25 @@
         """
         Returns the status of the RefreshSchemas operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_refresh_schemas_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_refresh_schemas_status)
         """
 
+    async def describe_replication_configs(
+        self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
+    ) -> DescribeReplicationConfigsResponseTypeDef:
+        """
+        Returns one or more existing DMS Serverless replication configurations as a list
+        of structures.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_configs)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replication_configs)
+        """
+
     async def describe_replication_instance_task_logs(
         self, *, ReplicationInstanceArn: str, MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeReplicationInstanceTaskLogsResponseTypeDef:
         """
         Returns information about the task logs for the specified task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_instance_task_logs)
@@ -770,14 +836,30 @@
         """
         Returns information about the replication subnet groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_subnet_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replication_subnet_groups)
         """
 
+    async def describe_replication_table_statistics(
+        self,
+        *,
+        ReplicationConfigArn: str,
+        MaxRecords: int = ...,
+        Marker: str = ...,
+        Filters: Sequence[FilterTypeDef] = ...
+    ) -> DescribeReplicationTableStatisticsResponseTypeDef:
+        """
+        Returns table and schema statistics for one or more provisioned replications
+        that use a given DMS Serverless replication configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_table_statistics)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replication_table_statistics)
+        """
+
     async def describe_replication_task_assessment_results(
         self, *, ReplicationTaskArn: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeReplicationTaskAssessmentResultsResponseTypeDef:
         """
         Returns the task assessment results from the Amazon S3 bucket that DMS creates
         in your Amazon Web Services account.
 
@@ -818,14 +900,25 @@
         Returns information about replication tasks for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replication_tasks)
         """
 
+    async def describe_replications(
+        self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
+    ) -> DescribeReplicationsResponseTypeDef:
+        """
+        Provides details on replication progress by returning status information for one
+        or more provisioned DMS Serverless replications.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replications)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replications)
+        """
+
     async def describe_schemas(
         self, *, EndpointArn: str, MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeSchemasResponseTypeDef:
         """
         Returns information about the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_schemas)
@@ -919,15 +1012,16 @@
         OracleSettings: OracleSettingsTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
-        GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
+        GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
+        TimestreamSettings: TimestreamSettingsTypeDef = ...
     ) -> ModifyEndpointResponseTypeDef:
         """
         Modifies the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_endpoint)
         """
@@ -944,14 +1038,35 @@
         """
         Modifies an existing DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_event_subscription)
         """
 
+    async def modify_replication_config(
+        self,
+        *,
+        ReplicationConfigArn: str,
+        ReplicationConfigIdentifier: str = ...,
+        ReplicationType: MigrationTypeValueType = ...,
+        TableMappings: str = ...,
+        ReplicationSettings: str = ...,
+        SupplementalSettings: str = ...,
+        ComputeConfig: ComputeConfigTypeDef = ...,
+        SourceEndpointArn: str = ...,
+        TargetEndpointArn: str = ...
+    ) -> ModifyReplicationConfigResponseTypeDef:
+        """
+        Modifies an existing DMS Serverless replication configuration that you can use
+        to start a replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_config)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_replication_config)
+        """
+
     async def modify_replication_instance(
         self,
         *,
         ReplicationInstanceArn: str,
         AllocatedStorage: int = ...,
         ApplyImmediately: bool = ...,
         ReplicationInstanceClass: str = ...,
@@ -1036,14 +1151,29 @@
         """
         Populates the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.refresh_schemas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#refresh_schemas)
         """
 
+    async def reload_replication_tables(
+        self,
+        *,
+        ReplicationConfigArn: str,
+        TablesToReload: Sequence[TableToReloadTypeDef],
+        ReloadOption: ReloadOptionValueType = ...
+    ) -> ReloadReplicationTablesResponseTypeDef:
+        """
+        Reloads the target database table with the source data for a given DMS
+        Serverless replication configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_replication_tables)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#reload_replication_tables)
+        """
+
     async def reload_tables(
         self,
         *,
         ReplicationTaskArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
         ReloadOption: ReloadOptionValueType = ...
     ) -> ReloadTablesResponseTypeDef:
@@ -1081,14 +1211,31 @@
         Starts the analysis of your source database to provide recommendations of target
         engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_recommendations)
         """
 
+    async def start_replication(
+        self,
+        *,
+        ReplicationConfigArn: str,
+        StartReplicationType: str,
+        CdcStartTime: TimestampTypeDef = ...,
+        CdcStartPosition: str = ...,
+        CdcStopPosition: str = ...
+    ) -> StartReplicationResponseTypeDef:
+        """
+        For a given DMS Serverless replication configuration, DMS connects to the source
+        endpoint and collects the metadata to analyze the replication workload.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_replication)
+        """
+
     async def start_replication_task(
         self,
         *,
         ReplicationTaskArn: str,
         StartReplicationTaskType: StartReplicationTaskTypeValueType,
         CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
@@ -1129,14 +1276,25 @@
         Starts a new premigration assessment run for one or more individual assessments
         of a migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_replication_task_assessment_run)
         """
 
+    async def stop_replication(
+        self, *, ReplicationConfigArn: str
+    ) -> StopReplicationResponseTypeDef:
+        """
+        For a given DMS Serverless replication configuration, DMS stops any and all
+        ongoing DMS Serverless replications.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#stop_replication)
+        """
+
     async def stop_replication_task(
         self, *, ReplicationTaskArn: str
     ) -> StopReplicationTaskResponseTypeDef:
         """
         Stops the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication_task)
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/client.pyi` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -43,51 +43,58 @@
     DescribeTableStatisticsPaginator,
 )
 from .type_defs import (
     ApplyPendingMaintenanceActionResponseTypeDef,
     BatchStartRecommendationsResponseTypeDef,
     BlobTypeDef,
     CancelReplicationTaskAssessmentRunResponseTypeDef,
+    ComputeConfigTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     CreateFleetAdvisorCollectorResponseTypeDef,
+    CreateReplicationConfigResponseTypeDef,
     CreateReplicationInstanceResponseTypeDef,
     CreateReplicationSubnetGroupResponseTypeDef,
     CreateReplicationTaskResponseTypeDef,
     DeleteCertificateResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     DeleteEndpointResponseTypeDef,
     DeleteEventSubscriptionResponseTypeDef,
     DeleteFleetAdvisorDatabasesResponseTypeDef,
+    DeleteReplicationConfigResponseTypeDef,
     DeleteReplicationInstanceResponseTypeDef,
     DeleteReplicationTaskAssessmentRunResponseTypeDef,
     DeleteReplicationTaskResponseTypeDef,
     DescribeAccountAttributesResponseTypeDef,
     DescribeApplicableIndividualAssessmentsResponseTypeDef,
     DescribeCertificatesResponseTypeDef,
     DescribeConnectionsResponseTypeDef,
     DescribeEndpointSettingsResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeEndpointTypesResponseTypeDef,
+    DescribeEngineVersionsResponseTypeDef,
     DescribeEventCategoriesResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeEventSubscriptionsResponseTypeDef,
     DescribeFleetAdvisorCollectorsResponseTypeDef,
     DescribeFleetAdvisorDatabasesResponseTypeDef,
     DescribeFleetAdvisorLsaAnalysisResponseTypeDef,
     DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef,
     DescribeFleetAdvisorSchemasResponseTypeDef,
     DescribeOrderableReplicationInstancesResponseTypeDef,
     DescribePendingMaintenanceActionsResponseTypeDef,
     DescribeRecommendationLimitationsResponseTypeDef,
     DescribeRecommendationsResponseTypeDef,
     DescribeRefreshSchemasStatusResponseTypeDef,
+    DescribeReplicationConfigsResponseTypeDef,
     DescribeReplicationInstancesResponseTypeDef,
     DescribeReplicationInstanceTaskLogsResponseTypeDef,
+    DescribeReplicationsResponseTypeDef,
     DescribeReplicationSubnetGroupsResponseTypeDef,
+    DescribeReplicationTableStatisticsResponseTypeDef,
     DescribeReplicationTaskAssessmentResultsResponseTypeDef,
     DescribeReplicationTaskAssessmentRunsResponseTypeDef,
     DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
     DescribeReplicationTasksResponseTypeDef,
     DescribeSchemasResponseTypeDef,
     DescribeTableStatisticsResponseTypeDef,
     DmsTransferSettingsTypeDef,
@@ -101,41 +108,46 @@
     ImportCertificateResponseTypeDef,
     KafkaSettingsTypeDef,
     KinesisSettingsTypeDef,
     ListTagsForResourceResponseTypeDef,
     MicrosoftSQLServerSettingsTypeDef,
     ModifyEndpointResponseTypeDef,
     ModifyEventSubscriptionResponseTypeDef,
+    ModifyReplicationConfigResponseTypeDef,
     ModifyReplicationInstanceResponseTypeDef,
     ModifyReplicationSubnetGroupResponseTypeDef,
     ModifyReplicationTaskResponseTypeDef,
     MongoDbSettingsTypeDef,
     MoveReplicationTaskResponseTypeDef,
     MySQLSettingsTypeDef,
     NeptuneSettingsTypeDef,
     OracleSettingsTypeDef,
     PostgreSQLSettingsTypeDef,
     RebootReplicationInstanceResponseTypeDef,
     RecommendationSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     RefreshSchemasResponseTypeDef,
+    ReloadReplicationTablesResponseTypeDef,
     ReloadTablesResponseTypeDef,
     RunFleetAdvisorLsaAnalysisResponseTypeDef,
     S3SettingsTypeDef,
     StartRecommendationsRequestEntryTypeDef,
+    StartReplicationResponseTypeDef,
     StartReplicationTaskAssessmentResponseTypeDef,
     StartReplicationTaskAssessmentRunResponseTypeDef,
     StartReplicationTaskResponseTypeDef,
+    StopReplicationResponseTypeDef,
     StopReplicationTaskResponseTypeDef,
     SybaseSettingsTypeDef,
     TableToReloadTypeDef,
     TagTypeDef,
     TestConnectionResponseTypeDef,
     TimestampTypeDef,
+    TimestreamSettingsTypeDef,
     UpdateSubscriptionsToEventBridgeResponseTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     ReplicationInstanceAvailableWaiter,
     ReplicationInstanceDeletedWaiter,
     ReplicationTaskDeletedWaiter,
@@ -288,15 +300,16 @@
         OracleSettings: OracleSettingsTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
-        GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
+        GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
+        TimestreamSettings: TimestreamSettingsTypeDef = ...
     ) -> CreateEndpointResponseTypeDef:
         """
         Creates an endpoint using the provided settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_endpoint)
         """
@@ -327,14 +340,35 @@
     ) -> CreateFleetAdvisorCollectorResponseTypeDef:
         """
         Creates a Fleet Advisor collector using the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_fleet_advisor_collector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_fleet_advisor_collector)
         """
+    async def create_replication_config(
+        self,
+        *,
+        ReplicationConfigIdentifier: str,
+        SourceEndpointArn: str,
+        TargetEndpointArn: str,
+        ComputeConfig: ComputeConfigTypeDef,
+        ReplicationType: MigrationTypeValueType,
+        TableMappings: str,
+        ReplicationSettings: str = ...,
+        SupplementalSettings: str = ...,
+        ResourceIdentifier: str = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> CreateReplicationConfigResponseTypeDef:
+        """
+        Creates a configuration that you can later provide to configure and start an DMS
+        Serverless replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.create_replication_config)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#create_replication_config)
+        """
     async def create_replication_instance(
         self,
         *,
         ReplicationInstanceIdentifier: str,
         ReplicationInstanceClass: str,
         AllocatedStorage: int = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
@@ -440,14 +474,23 @@
     ) -> DeleteFleetAdvisorDatabasesResponseTypeDef:
         """
         Deletes the specified Fleet Advisor collector databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_fleet_advisor_databases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#delete_fleet_advisor_databases)
         """
+    async def delete_replication_config(
+        self, *, ReplicationConfigArn: str
+    ) -> DeleteReplicationConfigResponseTypeDef:
+        """
+        Deletes an DMS Serverless replication configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_config)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#delete_replication_config)
+        """
     async def delete_replication_instance(
         self, *, ReplicationInstanceArn: str
     ) -> DeleteReplicationInstanceResponseTypeDef:
         """
         Deletes the specified replication instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.delete_replication_instance)
@@ -548,14 +591,23 @@
     ) -> DescribeEndpointsResponseTypeDef:
         """
         Returns information about the endpoints for your account in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_endpoints)
         """
+    async def describe_engine_versions(
+        self, *, MaxRecords: int = ..., Marker: str = ...
+    ) -> DescribeEngineVersionsResponseTypeDef:
+        """
+        Returns information about the replication instance versions used in the project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_engine_versions)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_engine_versions)
+        """
     async def describe_event_categories(
         self, *, SourceType: str = ..., Filters: Sequence[FilterTypeDef] = ...
     ) -> DescribeEventCategoriesResponseTypeDef:
         """
         Lists categories for all event source types, or, if specified, for a specified
         source type.
 
@@ -692,14 +744,24 @@
     ) -> DescribeRefreshSchemasStatusResponseTypeDef:
         """
         Returns the status of the RefreshSchemas operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_refresh_schemas_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_refresh_schemas_status)
         """
+    async def describe_replication_configs(
+        self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
+    ) -> DescribeReplicationConfigsResponseTypeDef:
+        """
+        Returns one or more existing DMS Serverless replication configurations as a list
+        of structures.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_configs)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replication_configs)
+        """
     async def describe_replication_instance_task_logs(
         self, *, ReplicationInstanceArn: str, MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeReplicationInstanceTaskLogsResponseTypeDef:
         """
         Returns information about the task logs for the specified task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_instance_task_logs)
@@ -720,14 +782,29 @@
     ) -> DescribeReplicationSubnetGroupsResponseTypeDef:
         """
         Returns information about the replication subnet groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_subnet_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replication_subnet_groups)
         """
+    async def describe_replication_table_statistics(
+        self,
+        *,
+        ReplicationConfigArn: str,
+        MaxRecords: int = ...,
+        Marker: str = ...,
+        Filters: Sequence[FilterTypeDef] = ...
+    ) -> DescribeReplicationTableStatisticsResponseTypeDef:
+        """
+        Returns table and schema statistics for one or more provisioned replications
+        that use a given DMS Serverless replication configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_table_statistics)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replication_table_statistics)
+        """
     async def describe_replication_task_assessment_results(
         self, *, ReplicationTaskArn: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeReplicationTaskAssessmentResultsResponseTypeDef:
         """
         Returns the task assessment results from the Amazon S3 bucket that DMS creates
         in your Amazon Web Services account.
 
@@ -764,14 +841,24 @@
         """
         Returns information about replication tasks for your account in the current
         region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replication_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replication_tasks)
         """
+    async def describe_replications(
+        self, *, Filters: Sequence[FilterTypeDef] = ..., MaxRecords: int = ..., Marker: str = ...
+    ) -> DescribeReplicationsResponseTypeDef:
+        """
+        Provides details on replication progress by returning status information for one
+        or more provisioned DMS Serverless replications.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_replications)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_replications)
+        """
     async def describe_schemas(
         self, *, EndpointArn: str, MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeSchemasResponseTypeDef:
         """
         Returns information about the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.describe_schemas)
@@ -860,15 +947,16 @@
         OracleSettings: OracleSettingsTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
-        GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
+        GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...,
+        TimestreamSettings: TimestreamSettingsTypeDef = ...
     ) -> ModifyEndpointResponseTypeDef:
         """
         Modifies the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_endpoint)
         """
@@ -883,14 +971,34 @@
     ) -> ModifyEventSubscriptionResponseTypeDef:
         """
         Modifies an existing DMS event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_event_subscription)
         """
+    async def modify_replication_config(
+        self,
+        *,
+        ReplicationConfigArn: str,
+        ReplicationConfigIdentifier: str = ...,
+        ReplicationType: MigrationTypeValueType = ...,
+        TableMappings: str = ...,
+        ReplicationSettings: str = ...,
+        SupplementalSettings: str = ...,
+        ComputeConfig: ComputeConfigTypeDef = ...,
+        SourceEndpointArn: str = ...,
+        TargetEndpointArn: str = ...
+    ) -> ModifyReplicationConfigResponseTypeDef:
+        """
+        Modifies an existing DMS Serverless replication configuration that you can use
+        to start a replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.modify_replication_config)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#modify_replication_config)
+        """
     async def modify_replication_instance(
         self,
         *,
         ReplicationInstanceArn: str,
         AllocatedStorage: int = ...,
         ApplyImmediately: bool = ...,
         ReplicationInstanceClass: str = ...,
@@ -969,14 +1077,28 @@
     ) -> RefreshSchemasResponseTypeDef:
         """
         Populates the schema for the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.refresh_schemas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#refresh_schemas)
         """
+    async def reload_replication_tables(
+        self,
+        *,
+        ReplicationConfigArn: str,
+        TablesToReload: Sequence[TableToReloadTypeDef],
+        ReloadOption: ReloadOptionValueType = ...
+    ) -> ReloadReplicationTablesResponseTypeDef:
+        """
+        Reloads the target database table with the source data for a given DMS
+        Serverless replication configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.reload_replication_tables)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#reload_replication_tables)
+        """
     async def reload_tables(
         self,
         *,
         ReplicationTaskArn: str,
         TablesToReload: Sequence[TableToReloadTypeDef],
         ReloadOption: ReloadOptionValueType = ...
     ) -> ReloadTablesResponseTypeDef:
@@ -1010,14 +1132,30 @@
         """
         Starts the analysis of your source database to provide recommendations of target
         engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_recommendations)
         """
+    async def start_replication(
+        self,
+        *,
+        ReplicationConfigArn: str,
+        StartReplicationType: str,
+        CdcStartTime: TimestampTypeDef = ...,
+        CdcStartPosition: str = ...,
+        CdcStopPosition: str = ...
+    ) -> StartReplicationResponseTypeDef:
+        """
+        For a given DMS Serverless replication configuration, DMS connects to the source
+        endpoint and collects the metadata to analyze the replication workload.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_replication)
+        """
     async def start_replication_task(
         self,
         *,
         ReplicationTaskArn: str,
         StartReplicationTaskType: StartReplicationTaskTypeValueType,
         CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
@@ -1055,14 +1193,24 @@
         """
         Starts a new premigration assessment run for one or more individual assessments
         of a migration task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task_assessment_run)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_replication_task_assessment_run)
         """
+    async def stop_replication(
+        self, *, ReplicationConfigArn: str
+    ) -> StopReplicationResponseTypeDef:
+        """
+        For a given DMS Serverless replication configuration, DMS stops any and all
+        ongoing DMS Serverless replications.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#stop_replication)
+        """
     async def stop_replication_task(
         self, *, ReplicationTaskArn: str
     ) -> StopReplicationTaskResponseTypeDef:
         """
         Stops the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.stop_replication_task)
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/literals.py` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "AuthMechanismValueType",
     "AuthTypeValueType",
     "CannedAclForObjectsValueType",
     "CharLengthSemanticsType",
     "CollectorStatusType",
     "CompressionTypeValueType",
     "DataFormatValueType",
+    "DatabaseModeType",
     "DatePartitionDelimiterValueType",
     "DatePartitionSequenceValueType",
     "DescribeCertificatesPaginatorName",
     "DescribeConnectionsPaginatorName",
     "DescribeEndpointTypesPaginatorName",
     "DescribeEndpointsPaginatorName",
     "DescribeEventSubscriptionsPaginatorName",
@@ -45,14 +46,16 @@
     "DmsSslModeValueType",
     "EncodingTypeValueType",
     "EncryptionModeValueType",
     "EndpointDeletedWaiterName",
     "EndpointSettingTypeValueType",
     "KafkaSaslMechanismType",
     "KafkaSecurityProtocolType",
+    "KafkaSslEndpointIdentificationAlgorithmType",
+    "LongVarcharMappingTypeType",
     "MessageFormatValueType",
     "MigrationTypeValueType",
     "NestingLevelValueType",
     "ParquetVersionValueType",
     "PluginNameValueType",
     "RedisAuthTypeValueType",
     "RefreshSchemasStatusTypeValueType",
@@ -94,14 +97,15 @@
     "public-read",
     "public-read-write",
 ]
 CharLengthSemanticsType = Literal["byte", "char", "default"]
 CollectorStatusType = Literal["ACTIVE", "UNREGISTERED"]
 CompressionTypeValueType = Literal["gzip", "none"]
 DataFormatValueType = Literal["csv", "parquet"]
+DatabaseModeType = Literal["babelfish", "default"]
 DatePartitionDelimiterValueType = Literal["DASH", "NONE", "SLASH", "UNDERSCORE"]
 DatePartitionSequenceValueType = Literal["DDMMYYYY", "MMYYYYDD", "YYYYMM", "YYYYMMDD", "YYYYMMDDHH"]
 DescribeCertificatesPaginatorName = Literal["describe_certificates"]
 DescribeConnectionsPaginatorName = Literal["describe_connections"]
 DescribeEndpointTypesPaginatorName = Literal["describe_endpoint_types"]
 DescribeEndpointsPaginatorName = Literal["describe_endpoints"]
 DescribeEventSubscriptionsPaginatorName = Literal["describe_event_subscriptions"]
@@ -120,14 +124,16 @@
 DmsSslModeValueType = Literal["none", "require", "verify-ca", "verify-full"]
 EncodingTypeValueType = Literal["plain", "plain-dictionary", "rle-dictionary"]
 EncryptionModeValueType = Literal["sse-kms", "sse-s3"]
 EndpointDeletedWaiterName = Literal["endpoint_deleted"]
 EndpointSettingTypeValueType = Literal["boolean", "enum", "integer", "string"]
 KafkaSaslMechanismType = Literal["plain", "scram-sha-512"]
 KafkaSecurityProtocolType = Literal["plaintext", "sasl-ssl", "ssl-authentication", "ssl-encryption"]
+KafkaSslEndpointIdentificationAlgorithmType = Literal["https", "none"]
+LongVarcharMappingTypeType = Literal["clob", "nclob", "wstring"]
 MessageFormatValueType = Literal["json", "json-unformatted"]
 MigrationTypeValueType = Literal["cdc", "full-load", "full-load-and-cdc"]
 NestingLevelValueType = Literal["none", "one"]
 ParquetVersionValueType = Literal["parquet-1-0", "parquet-2-0"]
 PluginNameValueType = Literal["no-preference", "pglogical", "test-decoding"]
 RedisAuthTypeValueType = Literal["auth-role", "auth-token", "none"]
 RefreshSchemasStatusTypeValueType = Literal["failed", "refreshing", "successful"]
@@ -166,14 +172,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -269,14 +276,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -355,26 +363,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
@@ -560,14 +570,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/literals.pyi` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "AuthMechanismValueType",
     "AuthTypeValueType",
     "CannedAclForObjectsValueType",
     "CharLengthSemanticsType",
     "CollectorStatusType",
     "CompressionTypeValueType",
     "DataFormatValueType",
+    "DatabaseModeType",
     "DatePartitionDelimiterValueType",
     "DatePartitionSequenceValueType",
     "DescribeCertificatesPaginatorName",
     "DescribeConnectionsPaginatorName",
     "DescribeEndpointTypesPaginatorName",
     "DescribeEndpointsPaginatorName",
     "DescribeEventSubscriptionsPaginatorName",
@@ -44,14 +45,16 @@
     "DmsSslModeValueType",
     "EncodingTypeValueType",
     "EncryptionModeValueType",
     "EndpointDeletedWaiterName",
     "EndpointSettingTypeValueType",
     "KafkaSaslMechanismType",
     "KafkaSecurityProtocolType",
+    "KafkaSslEndpointIdentificationAlgorithmType",
+    "LongVarcharMappingTypeType",
     "MessageFormatValueType",
     "MigrationTypeValueType",
     "NestingLevelValueType",
     "ParquetVersionValueType",
     "PluginNameValueType",
     "RedisAuthTypeValueType",
     "RefreshSchemasStatusTypeValueType",
@@ -92,14 +95,15 @@
     "public-read",
     "public-read-write",
 ]
 CharLengthSemanticsType = Literal["byte", "char", "default"]
 CollectorStatusType = Literal["ACTIVE", "UNREGISTERED"]
 CompressionTypeValueType = Literal["gzip", "none"]
 DataFormatValueType = Literal["csv", "parquet"]
+DatabaseModeType = Literal["babelfish", "default"]
 DatePartitionDelimiterValueType = Literal["DASH", "NONE", "SLASH", "UNDERSCORE"]
 DatePartitionSequenceValueType = Literal["DDMMYYYY", "MMYYYYDD", "YYYYMM", "YYYYMMDD", "YYYYMMDDHH"]
 DescribeCertificatesPaginatorName = Literal["describe_certificates"]
 DescribeConnectionsPaginatorName = Literal["describe_connections"]
 DescribeEndpointTypesPaginatorName = Literal["describe_endpoint_types"]
 DescribeEndpointsPaginatorName = Literal["describe_endpoints"]
 DescribeEventSubscriptionsPaginatorName = Literal["describe_event_subscriptions"]
@@ -118,14 +122,16 @@
 DmsSslModeValueType = Literal["none", "require", "verify-ca", "verify-full"]
 EncodingTypeValueType = Literal["plain", "plain-dictionary", "rle-dictionary"]
 EncryptionModeValueType = Literal["sse-kms", "sse-s3"]
 EndpointDeletedWaiterName = Literal["endpoint_deleted"]
 EndpointSettingTypeValueType = Literal["boolean", "enum", "integer", "string"]
 KafkaSaslMechanismType = Literal["plain", "scram-sha-512"]
 KafkaSecurityProtocolType = Literal["plaintext", "sasl-ssl", "ssl-authentication", "ssl-encryption"]
+KafkaSslEndpointIdentificationAlgorithmType = Literal["https", "none"]
+LongVarcharMappingTypeType = Literal["clob", "nclob", "wstring"]
 MessageFormatValueType = Literal["json", "json-unformatted"]
 MigrationTypeValueType = Literal["cdc", "full-load", "full-load-and-cdc"]
 NestingLevelValueType = Literal["none", "one"]
 ParquetVersionValueType = Literal["parquet-1-0", "parquet-2-0"]
 PluginNameValueType = Literal["no-preference", "pglogical", "test-decoding"]
 RedisAuthTypeValueType = Literal["auth-role", "auth-token", "none"]
 RefreshSchemasStatusTypeValueType = Literal["failed", "refreshing", "successful"]
@@ -164,14 +170,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -267,14 +274,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -353,26 +361,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
@@ -558,14 +568,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/paginator.py` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/paginator.pyi` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/type_defs.py` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,23 +20,26 @@
 from .literals import (
     AuthMechanismValueType,
     AuthTypeValueType,
     CannedAclForObjectsValueType,
     CharLengthSemanticsType,
     CollectorStatusType,
     CompressionTypeValueType,
+    DatabaseModeType,
     DataFormatValueType,
     DatePartitionDelimiterValueType,
     DatePartitionSequenceValueType,
     DmsSslModeValueType,
     EncodingTypeValueType,
     EncryptionModeValueType,
     EndpointSettingTypeValueType,
     KafkaSaslMechanismType,
     KafkaSecurityProtocolType,
+    KafkaSslEndpointIdentificationAlgorithmType,
+    LongVarcharMappingTypeType,
     MessageFormatValueType,
     MigrationTypeValueType,
     NestingLevelValueType,
     ParquetVersionValueType,
     PluginNameValueType,
     RedisAuthTypeValueType,
     RefreshSchemasStatusTypeValueType,
@@ -70,14 +73,15 @@
     "BatchStartRecommendationsErrorEntryTypeDef",
     "BlobTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     "CertificateTypeDef",
     "CollectorHealthCheckTypeDef",
     "InventoryDataTypeDef",
     "CollectorShortInfoResponseTypeDef",
+    "ComputeConfigTypeDef",
     "ConnectionTypeDef",
     "DmsTransferSettingsTypeDef",
     "DocDbSettingsTypeDef",
     "DynamoDbSettingsTypeDef",
     "ElasticsearchSettingsTypeDef",
     "GcpMySQLSettingsTypeDef",
     "IBMDb2SettingsTypeDef",
@@ -89,110 +93,122 @@
     "NeptuneSettingsTypeDef",
     "OracleSettingsTypeDef",
     "PostgreSQLSettingsTypeDef",
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
+    "TimestreamSettingsTypeDef",
     "EventSubscriptionTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
     "TimestampTypeDef",
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     "ServerShortInfoResponseTypeDef",
     "DatabaseShortInfoResponseTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
+    "DeleteReplicationConfigMessageRequestTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
     "EndpointSettingTypeDef",
     "SupportedEndpointTypeTypeDef",
+    "DescribeEngineVersionsMessageRequestTypeDef",
+    "EngineVersionTypeDef",
     "EventCategoryGroupTypeDef",
     "EventTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
     "FleetAdvisorLsaAnalysisResponseTypeDef",
     "FleetAdvisorSchemaObjectResponseTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     "OrderableReplicationInstanceTypeDef",
     "LimitationTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     "RefreshSchemasStatusTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     "ReplicationInstanceTaskLogTypeDef",
+    "TableStatisticsTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     "ReplicationTaskAssessmentResultTypeDef",
     "ReplicationTaskIndividualAssessmentTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
-    "TableStatisticsTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
     "PendingMaintenanceActionTypeDef",
+    "ProvisionDataTypeDef",
     "RdsConfigurationTypeDef",
     "RdsRequirementsTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "ReplicationPendingModifiedValuesTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
+    "ReplicationStatsTypeDef",
     "ReplicationTaskAssessmentRunProgressTypeDef",
     "ReplicationTaskStatsTypeDef",
     "SchemaShortInfoResponseTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
+    "StopReplicationMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
     "CreateFleetAdvisorCollectorResponseTypeDef",
     "DeleteFleetAdvisorDatabasesResponseTypeDef",
     "DescribeAccountAttributesResponseTypeDef",
     "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     "DescribeSchemasResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ReloadReplicationTablesResponseTypeDef",
     "ReloadTablesResponseTypeDef",
     "RunFleetAdvisorLsaAnalysisResponseTypeDef",
     "UpdateSubscriptionsToEventBridgeResponseTypeDef",
     "SubnetTypeDef",
     "BatchStartRecommendationsResponseTypeDef",
     "ImportCertificateMessageRequestTypeDef",
     "DeleteCertificateResponseTypeDef",
     "DescribeCertificatesResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "CollectorResponseTypeDef",
+    "CreateReplicationConfigMessageRequestTypeDef",
+    "ModifyReplicationConfigMessageRequestTypeDef",
+    "ReplicationConfigTypeDef",
     "DeleteConnectionResponseTypeDef",
     "DescribeConnectionsResponseTypeDef",
     "TestConnectionResponseTypeDef",
     "CreateEndpointMessageRequestTypeDef",
     "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
     "CreateEventSubscriptionResponseTypeDef",
     "DeleteEventSubscriptionResponseTypeDef",
     "DescribeEventSubscriptionsResponseTypeDef",
     "ModifyEventSubscriptionResponseTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
+    "StartReplicationMessageRequestTypeDef",
     "StartReplicationTaskMessageRequestTypeDef",
     "DatabaseResponseTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
     "DescribeEndpointsMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
@@ -201,19 +217,22 @@
     "DescribeFleetAdvisorCollectorsRequestRequestTypeDef",
     "DescribeFleetAdvisorDatabasesRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemasRequestRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "DescribeRecommendationLimitationsRequestRequestTypeDef",
     "DescribeRecommendationsRequestRequestTypeDef",
+    "DescribeReplicationConfigsMessageRequestTypeDef",
     "DescribeReplicationInstancesMessageRequestTypeDef",
     "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
+    "DescribeReplicationTableStatisticsMessageRequestTypeDef",
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
     "DescribeReplicationTasksMessageRequestTypeDef",
+    "DescribeReplicationsMessageRequestTypeDef",
     "DescribeTableStatisticsMessageRequestTypeDef",
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
@@ -230,45 +249,56 @@
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef",
     "DescribeEndpointSettingsResponseTypeDef",
     "DescribeEndpointTypesResponseTypeDef",
+    "DescribeEngineVersionsResponseTypeDef",
     "DescribeEventCategoriesResponseTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
     "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
     "DescribeOrderableReplicationInstancesResponseTypeDef",
     "DescribeRecommendationLimitationsResponseTypeDef",
     "DescribeRefreshSchemasStatusResponseTypeDef",
     "RefreshSchemasResponseTypeDef",
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
+    "DescribeReplicationTableStatisticsResponseTypeDef",
+    "DescribeTableStatisticsResponseTypeDef",
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
-    "DescribeTableStatisticsResponseTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "RdsRecommendationTypeDef",
     "StartRecommendationsRequestEntryTypeDef",
     "StartRecommendationsRequestRequestTypeDef",
+    "ReloadReplicationTablesMessageRequestTypeDef",
     "ReloadTablesMessageRequestTypeDef",
+    "ReplicationTypeDef",
     "ReplicationTaskAssessmentRunTypeDef",
     "ReplicationTaskTypeDef",
     "SchemaResponseTypeDef",
     "ReplicationSubnetGroupTypeDef",
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
+    "CreateReplicationConfigResponseTypeDef",
+    "DeleteReplicationConfigResponseTypeDef",
+    "DescribeReplicationConfigsResponseTypeDef",
+    "ModifyReplicationConfigResponseTypeDef",
     "CreateEndpointResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ModifyEndpointResponseTypeDef",
     "DescribeFleetAdvisorDatabasesResponseTypeDef",
     "ApplyPendingMaintenanceActionResponseTypeDef",
     "DescribePendingMaintenanceActionsResponseTypeDef",
     "RecommendationDataTypeDef",
     "BatchStartRecommendationsRequestRequestTypeDef",
+    "DescribeReplicationsResponseTypeDef",
+    "StartReplicationResponseTypeDef",
+    "StopReplicationResponseTypeDef",
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
     "StartReplicationTaskAssessmentRunResponseTypeDef",
     "CreateReplicationTaskResponseTypeDef",
     "DeleteReplicationTaskResponseTypeDef",
     "DescribeReplicationTasksResponseTypeDef",
@@ -399,14 +429,30 @@
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
     },
     total=False,
 )
 
+ComputeConfigTypeDef = TypedDict(
+    "ComputeConfigTypeDef",
+    {
+        "AvailabilityZone": str,
+        "DnsNameServers": str,
+        "KmsKeyId": str,
+        "MaxCapacityUnits": int,
+        "MinCapacityUnits": int,
+        "MultiAZ": bool,
+        "PreferredMaintenanceWindow": str,
+        "ReplicationSubnetGroupId": str,
+        "VpcSecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ReplicationInstanceArn": str,
         "EndpointArn": str,
         "Status": str,
         "LastFailureMessage": str,
@@ -435,14 +481,16 @@
         "DatabaseName": str,
         "NestingLevel": NestingLevelValueType,
         "ExtractDocId": bool,
         "DocsToInvestigate": int,
         "KmsKeyId": str,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
+        "UseUpdateLookUp": bool,
+        "ReplicateShardCollections": bool,
     },
     total=False,
 )
 
 DynamoDbSettingsTypeDef = TypedDict(
     "DynamoDbSettingsTypeDef",
     {
@@ -530,14 +578,15 @@
         "SslClientKeyArn": str,
         "SslClientKeyPassword": str,
         "SslCaCertificateArn": str,
         "SaslUsername": str,
         "SaslPassword": str,
         "NoHexPrefix": bool,
         "SaslMechanism": KafkaSaslMechanismType,
+        "SslEndpointIdentificationAlgorithm": KafkaSslEndpointIdentificationAlgorithmType,
     },
     total=False,
 )
 
 KinesisSettingsTypeDef = TypedDict(
     "KinesisSettingsTypeDef",
     {
@@ -592,14 +641,16 @@
         "NestingLevel": NestingLevelValueType,
         "ExtractDocId": str,
         "DocsToInvestigate": str,
         "AuthSource": str,
         "KmsKeyId": str,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
+        "UseUpdateLookUp": bool,
+        "ReplicateShardCollections": bool,
     },
     total=False,
 )
 
 MySQLSettingsTypeDef = TypedDict(
     "MySQLSettingsTypeDef",
     {
@@ -686,14 +737,15 @@
         "UseLogminerReader": bool,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
         "SecretsManagerOracleAsmAccessRoleArn": str,
         "SecretsManagerOracleAsmSecretId": str,
         "TrimSpaceInChar": bool,
         "ConvertTimestampWithZoneToUTC": bool,
+        "OpenTransactionWindow": int,
     },
     total=False,
 )
 
 PostgreSQLSettingsTypeDef = TypedDict(
     "PostgreSQLSettingsTypeDef",
     {
@@ -713,14 +765,18 @@
         "Username": str,
         "SlotName": str,
         "PluginName": PluginNameValueType,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
         "TrimSpaceInChar": bool,
         "MapBooleanAsBoolean": bool,
+        "MapJsonbAsClob": bool,
+        "MapLongVarcharAs": LongVarcharMappingTypeType,
+        "DatabaseMode": DatabaseModeType,
+        "BabelfishDatabaseName": str,
     },
     total=False,
 )
 
 _RequiredRedisSettingsTypeDef = TypedDict(
     "_RequiredRedisSettingsTypeDef",
     {
@@ -841,14 +897,38 @@
         "Username": str,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
     },
     total=False,
 )
 
+_RequiredTimestreamSettingsTypeDef = TypedDict(
+    "_RequiredTimestreamSettingsTypeDef",
+    {
+        "DatabaseName": str,
+        "MemoryDuration": int,
+        "MagneticDuration": int,
+    },
+)
+_OptionalTimestreamSettingsTypeDef = TypedDict(
+    "_OptionalTimestreamSettingsTypeDef",
+    {
+        "CdcInsertsAndUpdates": bool,
+        "EnableMagneticStoreWrites": bool,
+    },
+    total=False,
+)
+
+
+class TimestreamSettingsTypeDef(
+    _RequiredTimestreamSettingsTypeDef, _OptionalTimestreamSettingsTypeDef
+):
+    pass
+
+
 EventSubscriptionTypeDef = TypedDict(
     "EventSubscriptionTypeDef",
     {
         "CustomerAwsId": str,
         "CustSubscriptionId": str,
         "SnsTopicArn": str,
         "Status": str,
@@ -960,14 +1040,21 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
+DeleteReplicationConfigMessageRequestTypeDef = TypedDict(
+    "DeleteReplicationConfigMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+    },
+)
+
 DeleteReplicationInstanceMessageRequestTypeDef = TypedDict(
     "DeleteReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
 )
 
@@ -1080,14 +1167,38 @@
         "EndpointType": ReplicationEndpointTypeValueType,
         "ReplicationInstanceEngineMinimumVersion": str,
         "EngineDisplayName": str,
     },
     total=False,
 )
 
+DescribeEngineVersionsMessageRequestTypeDef = TypedDict(
+    "DescribeEngineVersionsMessageRequestTypeDef",
+    {
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+EngineVersionTypeDef = TypedDict(
+    "EngineVersionTypeDef",
+    {
+        "Version": str,
+        "Lifecycle": str,
+        "ReleaseStatus": ReleaseStatusValuesType,
+        "LaunchDate": datetime,
+        "AutoUpgradeDate": datetime,
+        "DeprecationDate": datetime,
+        "ForceUpgradeDate": datetime,
+        "AvailableUpgrades": List[str],
+    },
+    total=False,
+)
+
 EventCategoryGroupTypeDef = TypedDict(
     "EventCategoryGroupTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
     total=False,
@@ -1221,14 +1332,44 @@
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
     total=False,
 )
 
+TableStatisticsTypeDef = TypedDict(
+    "TableStatisticsTypeDef",
+    {
+        "SchemaName": str,
+        "TableName": str,
+        "Inserts": int,
+        "Deletes": int,
+        "Updates": int,
+        "Ddls": int,
+        "AppliedInserts": int,
+        "AppliedDeletes": int,
+        "AppliedUpdates": int,
+        "AppliedDdls": int,
+        "FullLoadRows": int,
+        "FullLoadCondtnlChkFailedRows": int,
+        "FullLoadErrorRows": int,
+        "FullLoadStartTime": datetime,
+        "FullLoadEndTime": datetime,
+        "FullLoadReloaded": bool,
+        "LastUpdateTime": datetime,
+        "TableState": str,
+        "ValidationPendingRecords": int,
+        "ValidationFailedRecords": int,
+        "ValidationSuspendedRecords": int,
+        "ValidationState": str,
+        "ValidationStateDetails": str,
+    },
+    total=False,
+)
+
 DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1279,44 +1420,14 @@
 
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
 
-TableStatisticsTypeDef = TypedDict(
-    "TableStatisticsTypeDef",
-    {
-        "SchemaName": str,
-        "TableName": str,
-        "Inserts": int,
-        "Deletes": int,
-        "Updates": int,
-        "Ddls": int,
-        "AppliedInserts": int,
-        "AppliedDeletes": int,
-        "AppliedUpdates": int,
-        "AppliedDdls": int,
-        "FullLoadRows": int,
-        "FullLoadCondtnlChkFailedRows": int,
-        "FullLoadErrorRows": int,
-        "FullLoadStartTime": datetime,
-        "FullLoadEndTime": datetime,
-        "FullLoadReloaded": bool,
-        "LastUpdateTime": datetime,
-        "TableState": str,
-        "ValidationPendingRecords": int,
-        "ValidationFailedRecords": int,
-        "ValidationSuspendedRecords": int,
-        "ValidationState": str,
-        "ValidationStateDetails": str,
-    },
-    total=False,
-)
-
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
     },
     total=False,
@@ -1419,38 +1530,53 @@
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
     total=False,
 )
 
+ProvisionDataTypeDef = TypedDict(
+    "ProvisionDataTypeDef",
+    {
+        "ProvisionState": str,
+        "ProvisionedCapacityUnits": int,
+        "DateProvisioned": datetime,
+        "IsNewProvisioningAvailable": bool,
+        "DateNewProvisioningDataAvailable": datetime,
+        "ReasonForNewProvisioningData": str,
+    },
+    total=False,
+)
+
 RdsConfigurationTypeDef = TypedDict(
     "RdsConfigurationTypeDef",
     {
         "EngineEdition": str,
         "InstanceType": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageType": str,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
+        "EngineVersion": str,
     },
     total=False,
 )
 
 RdsRequirementsTypeDef = TypedDict(
     "RdsRequirementsTypeDef",
     {
         "EngineEdition": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
+        "EngineVersion": str,
     },
     total=False,
 )
 
 _RequiredRebootReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredRebootReplicationInstanceMessageRequestTypeDef",
     {
@@ -1523,14 +1649,32 @@
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
     total=False,
 )
 
+ReplicationStatsTypeDef = TypedDict(
+    "ReplicationStatsTypeDef",
+    {
+        "FullLoadProgressPercent": int,
+        "ElapsedTimeMillis": int,
+        "TablesLoaded": int,
+        "TablesLoading": int,
+        "TablesQueued": int,
+        "TablesErrored": int,
+        "FreshStartDate": datetime,
+        "StartDate": datetime,
+        "StopDate": datetime,
+        "FullLoadStartDate": datetime,
+        "FullLoadFinishDate": datetime,
+    },
+    total=False,
+)
+
 ReplicationTaskAssessmentRunProgressTypeDef = TypedDict(
     "ReplicationTaskAssessmentRunProgressTypeDef",
     {
         "IndividualAssessmentCount": int,
         "IndividualAssessmentCompletedCount": int,
     },
     total=False,
@@ -1598,14 +1742,21 @@
 class StartReplicationTaskAssessmentRunMessageRequestTypeDef(
     _RequiredStartReplicationTaskAssessmentRunMessageRequestTypeDef,
     _OptionalStartReplicationTaskAssessmentRunMessageRequestTypeDef,
 ):
     pass
 
 
+StopReplicationMessageRequestTypeDef = TypedDict(
+    "StopReplicationMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+    },
+)
+
 StopReplicationTaskMessageRequestTypeDef = TypedDict(
     "StopReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
 
@@ -1778,14 +1929,22 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReloadReplicationTablesResponseTypeDef = TypedDict(
+    "ReloadReplicationTablesResponseTypeDef",
+    {
+        "ReplicationConfigArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ReloadTablesResponseTypeDef = TypedDict(
     "ReloadTablesResponseTypeDef",
     {
         "ReplicationTaskArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1889,14 +2048,91 @@
         "CreatedDate": str,
         "ModifiedDate": str,
         "InventoryData": InventoryDataTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateReplicationConfigMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateReplicationConfigMessageRequestTypeDef",
+    {
+        "ReplicationConfigIdentifier": str,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+        "ComputeConfig": ComputeConfigTypeDef,
+        "ReplicationType": MigrationTypeValueType,
+        "TableMappings": str,
+    },
+)
+_OptionalCreateReplicationConfigMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateReplicationConfigMessageRequestTypeDef",
+    {
+        "ReplicationSettings": str,
+        "SupplementalSettings": str,
+        "ResourceIdentifier": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateReplicationConfigMessageRequestTypeDef(
+    _RequiredCreateReplicationConfigMessageRequestTypeDef,
+    _OptionalCreateReplicationConfigMessageRequestTypeDef,
+):
+    pass
+
+
+_RequiredModifyReplicationConfigMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyReplicationConfigMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+    },
+)
+_OptionalModifyReplicationConfigMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyReplicationConfigMessageRequestTypeDef",
+    {
+        "ReplicationConfigIdentifier": str,
+        "ReplicationType": MigrationTypeValueType,
+        "TableMappings": str,
+        "ReplicationSettings": str,
+        "SupplementalSettings": str,
+        "ComputeConfig": ComputeConfigTypeDef,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+    },
+    total=False,
+)
+
+
+class ModifyReplicationConfigMessageRequestTypeDef(
+    _RequiredModifyReplicationConfigMessageRequestTypeDef,
+    _OptionalModifyReplicationConfigMessageRequestTypeDef,
+):
+    pass
+
+
+ReplicationConfigTypeDef = TypedDict(
+    "ReplicationConfigTypeDef",
+    {
+        "ReplicationConfigIdentifier": str,
+        "ReplicationConfigArn": str,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+        "ReplicationType": MigrationTypeValueType,
+        "ComputeConfig": ComputeConfigTypeDef,
+        "ReplicationSettings": str,
+        "SupplementalSettings": str,
+        "TableMappings": str,
+        "ReplicationConfigCreateTime": datetime,
+        "ReplicationConfigUpdateTime": datetime,
+    },
+    total=False,
+)
+
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1956,14 +2192,15 @@
         "SybaseSettings": SybaseSettingsTypeDef,
         "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
         "IBMDb2Settings": IBMDb2SettingsTypeDef,
         "ResourceIdentifier": str,
         "DocDbSettings": DocDbSettingsTypeDef,
         "RedisSettings": RedisSettingsTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
+        "TimestreamSettings": TimestreamSettingsTypeDef,
     },
     total=False,
 )
 
 
 class CreateEndpointMessageRequestTypeDef(
     _RequiredCreateEndpointMessageRequestTypeDef, _OptionalCreateEndpointMessageRequestTypeDef
@@ -2005,14 +2242,15 @@
         "OracleSettings": OracleSettingsTypeDef,
         "SybaseSettings": SybaseSettingsTypeDef,
         "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
         "IBMDb2Settings": IBMDb2SettingsTypeDef,
         "DocDbSettings": DocDbSettingsTypeDef,
         "RedisSettings": RedisSettingsTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
+        "TimestreamSettings": TimestreamSettingsTypeDef,
     },
     total=False,
 )
 
 _RequiredModifyEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointMessageRequestTypeDef",
     {
@@ -2050,14 +2288,15 @@
         "SybaseSettings": SybaseSettingsTypeDef,
         "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
         "IBMDb2Settings": IBMDb2SettingsTypeDef,
         "DocDbSettings": DocDbSettingsTypeDef,
         "RedisSettings": RedisSettingsTypeDef,
         "ExactSettings": bool,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
+        "TimestreamSettings": TimestreamSettingsTypeDef,
     },
     total=False,
 )
 
 
 class ModifyEndpointMessageRequestTypeDef(
     _RequiredModifyEndpointMessageRequestTypeDef, _OptionalModifyEndpointMessageRequestTypeDef
@@ -2156,14 +2395,38 @@
 class ModifyReplicationTaskMessageRequestTypeDef(
     _RequiredModifyReplicationTaskMessageRequestTypeDef,
     _OptionalModifyReplicationTaskMessageRequestTypeDef,
 ):
     pass
 
 
+_RequiredStartReplicationMessageRequestTypeDef = TypedDict(
+    "_RequiredStartReplicationMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+        "StartReplicationType": str,
+    },
+)
+_OptionalStartReplicationMessageRequestTypeDef = TypedDict(
+    "_OptionalStartReplicationMessageRequestTypeDef",
+    {
+        "CdcStartTime": TimestampTypeDef,
+        "CdcStartPosition": str,
+        "CdcStopPosition": str,
+    },
+    total=False,
+)
+
+
+class StartReplicationMessageRequestTypeDef(
+    _RequiredStartReplicationMessageRequestTypeDef, _OptionalStartReplicationMessageRequestTypeDef
+):
+    pass
+
+
 _RequiredStartReplicationTaskMessageRequestTypeDef = TypedDict(
     "_RequiredStartReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "StartReplicationTaskType": StartReplicationTaskTypeValueType,
     },
 )
@@ -2342,14 +2605,24 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeReplicationConfigsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationConfigsMessageRequestTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
 DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
     "DescribeReplicationInstancesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2362,14 +2635,38 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredDescribeReplicationTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeReplicationTableStatisticsMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+    },
+)
+_OptionalDescribeReplicationTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeReplicationTableStatisticsMessageRequestTypeDef",
+    {
+        "MaxRecords": int,
+        "Marker": str,
+        "Filters": Sequence[FilterTypeDef],
+    },
+    total=False,
+)
+
+
+class DescribeReplicationTableStatisticsMessageRequestTypeDef(
+    _RequiredDescribeReplicationTableStatisticsMessageRequestTypeDef,
+    _OptionalDescribeReplicationTableStatisticsMessageRequestTypeDef,
+):
+    pass
+
+
 DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2393,14 +2690,24 @@
         "MaxRecords": int,
         "Marker": str,
         "WithoutSettings": bool,
     },
     total=False,
 )
 
+DescribeReplicationsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationsMessageRequestTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
 _RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
 _OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
@@ -2678,14 +2985,23 @@
     {
         "Marker": str,
         "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeEngineVersionsResponseTypeDef = TypedDict(
+    "DescribeEngineVersionsResponseTypeDef",
+    {
+        "EngineVersions": List[EngineVersionTypeDef],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeEventCategoriesResponseTypeDef = TypedDict(
     "DescribeEventCategoriesResponseTypeDef",
     {
         "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2757,14 +3073,34 @@
         "ReplicationInstanceArn": str,
         "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeReplicationTableStatisticsResponseTypeDef = TypedDict(
+    "DescribeReplicationTableStatisticsResponseTypeDef",
+    {
+        "ReplicationConfigArn": str,
+        "Marker": str,
+        "ReplicationTableStatistics": List[TableStatisticsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTableStatisticsResponseTypeDef = TypedDict(
+    "DescribeTableStatisticsResponseTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "TableStatistics": List[TableStatisticsTypeDef],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     {
         "Marker": str,
         "BucketName": str,
         "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2776,24 +3112,14 @@
     {
         "Marker": str,
         "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeTableStatisticsResponseTypeDef = TypedDict(
-    "DescribeTableStatisticsResponseTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "TableStatistics": List[TableStatisticsTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -2820,14 +3146,37 @@
     "StartRecommendationsRequestRequestTypeDef",
     {
         "DatabaseId": str,
         "Settings": RecommendationSettingsTypeDef,
     },
 )
 
+_RequiredReloadReplicationTablesMessageRequestTypeDef = TypedDict(
+    "_RequiredReloadReplicationTablesMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+        "TablesToReload": Sequence[TableToReloadTypeDef],
+    },
+)
+_OptionalReloadReplicationTablesMessageRequestTypeDef = TypedDict(
+    "_OptionalReloadReplicationTablesMessageRequestTypeDef",
+    {
+        "ReloadOption": ReloadOptionValueType,
+    },
+    total=False,
+)
+
+
+class ReloadReplicationTablesMessageRequestTypeDef(
+    _RequiredReloadReplicationTablesMessageRequestTypeDef,
+    _OptionalReloadReplicationTablesMessageRequestTypeDef,
+):
+    pass
+
+
 _RequiredReloadTablesMessageRequestTypeDef = TypedDict(
     "_RequiredReloadTablesMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TablesToReload": Sequence[TableToReloadTypeDef],
     },
 )
@@ -2842,14 +3191,39 @@
 
 class ReloadTablesMessageRequestTypeDef(
     _RequiredReloadTablesMessageRequestTypeDef, _OptionalReloadTablesMessageRequestTypeDef
 ):
     pass
 
 
+ReplicationTypeDef = TypedDict(
+    "ReplicationTypeDef",
+    {
+        "ReplicationConfigIdentifier": str,
+        "ReplicationConfigArn": str,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+        "ReplicationType": MigrationTypeValueType,
+        "Status": str,
+        "ProvisionData": ProvisionDataTypeDef,
+        "StopReason": str,
+        "FailureMessages": List[str],
+        "ReplicationStats": ReplicationStatsTypeDef,
+        "StartReplicationType": str,
+        "CdcStartTime": datetime,
+        "CdcStartPosition": str,
+        "CdcStopPosition": str,
+        "RecoveryCheckpoint": str,
+        "ReplicationCreateTime": datetime,
+        "ReplicationUpdateTime": datetime,
+        "ReplicationLastStopTime": datetime,
+    },
+    total=False,
+)
+
 ReplicationTaskAssessmentRunTypeDef = TypedDict(
     "ReplicationTaskAssessmentRunTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
         "ReplicationTaskArn": str,
         "Status": str,
         "ReplicationTaskAssessmentRunCreationDate": datetime,
@@ -2925,14 +3299,47 @@
     {
         "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateReplicationConfigResponseTypeDef = TypedDict(
+    "CreateReplicationConfigResponseTypeDef",
+    {
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteReplicationConfigResponseTypeDef = TypedDict(
+    "DeleteReplicationConfigResponseTypeDef",
+    {
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReplicationConfigsResponseTypeDef = TypedDict(
+    "DescribeReplicationConfigsResponseTypeDef",
+    {
+        "Marker": str,
+        "ReplicationConfigs": List[ReplicationConfigTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyReplicationConfigResponseTypeDef = TypedDict(
+    "ModifyReplicationConfigResponseTypeDef",
+    {
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3000,14 +3407,39 @@
     "BatchStartRecommendationsRequestRequestTypeDef",
     {
         "Data": Sequence[StartRecommendationsRequestEntryTypeDef],
     },
     total=False,
 )
 
+DescribeReplicationsResponseTypeDef = TypedDict(
+    "DescribeReplicationsResponseTypeDef",
+    {
+        "Marker": str,
+        "Replications": List[ReplicationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReplicationResponseTypeDef = TypedDict(
+    "StartReplicationResponseTypeDef",
+    {
+        "Replication": ReplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopReplicationResponseTypeDef = TypedDict(
+    "StopReplicationResponseTypeDef",
+    {
+        "Replication": ReplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/type_defs.pyi` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -20,23 +20,26 @@
 from .literals import (
     AuthMechanismValueType,
     AuthTypeValueType,
     CannedAclForObjectsValueType,
     CharLengthSemanticsType,
     CollectorStatusType,
     CompressionTypeValueType,
+    DatabaseModeType,
     DataFormatValueType,
     DatePartitionDelimiterValueType,
     DatePartitionSequenceValueType,
     DmsSslModeValueType,
     EncodingTypeValueType,
     EncryptionModeValueType,
     EndpointSettingTypeValueType,
     KafkaSaslMechanismType,
     KafkaSecurityProtocolType,
+    KafkaSslEndpointIdentificationAlgorithmType,
+    LongVarcharMappingTypeType,
     MessageFormatValueType,
     MigrationTypeValueType,
     NestingLevelValueType,
     ParquetVersionValueType,
     PluginNameValueType,
     RedisAuthTypeValueType,
     RefreshSchemasStatusTypeValueType,
@@ -69,14 +72,15 @@
     "BatchStartRecommendationsErrorEntryTypeDef",
     "BlobTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     "CertificateTypeDef",
     "CollectorHealthCheckTypeDef",
     "InventoryDataTypeDef",
     "CollectorShortInfoResponseTypeDef",
+    "ComputeConfigTypeDef",
     "ConnectionTypeDef",
     "DmsTransferSettingsTypeDef",
     "DocDbSettingsTypeDef",
     "DynamoDbSettingsTypeDef",
     "ElasticsearchSettingsTypeDef",
     "GcpMySQLSettingsTypeDef",
     "IBMDb2SettingsTypeDef",
@@ -88,110 +92,122 @@
     "NeptuneSettingsTypeDef",
     "OracleSettingsTypeDef",
     "PostgreSQLSettingsTypeDef",
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
+    "TimestreamSettingsTypeDef",
     "EventSubscriptionTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
     "TimestampTypeDef",
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     "ServerShortInfoResponseTypeDef",
     "DatabaseShortInfoResponseTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
+    "DeleteReplicationConfigMessageRequestTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
     "EndpointSettingTypeDef",
     "SupportedEndpointTypeTypeDef",
+    "DescribeEngineVersionsMessageRequestTypeDef",
+    "EngineVersionTypeDef",
     "EventCategoryGroupTypeDef",
     "EventTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
     "FleetAdvisorLsaAnalysisResponseTypeDef",
     "FleetAdvisorSchemaObjectResponseTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     "OrderableReplicationInstanceTypeDef",
     "LimitationTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     "RefreshSchemasStatusTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     "ReplicationInstanceTaskLogTypeDef",
+    "TableStatisticsTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     "ReplicationTaskAssessmentResultTypeDef",
     "ReplicationTaskIndividualAssessmentTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
-    "TableStatisticsTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
     "PendingMaintenanceActionTypeDef",
+    "ProvisionDataTypeDef",
     "RdsConfigurationTypeDef",
     "RdsRequirementsTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "ReplicationPendingModifiedValuesTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
+    "ReplicationStatsTypeDef",
     "ReplicationTaskAssessmentRunProgressTypeDef",
     "ReplicationTaskStatsTypeDef",
     "SchemaShortInfoResponseTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
+    "StopReplicationMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
     "CreateFleetAdvisorCollectorResponseTypeDef",
     "DeleteFleetAdvisorDatabasesResponseTypeDef",
     "DescribeAccountAttributesResponseTypeDef",
     "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     "DescribeSchemasResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ReloadReplicationTablesResponseTypeDef",
     "ReloadTablesResponseTypeDef",
     "RunFleetAdvisorLsaAnalysisResponseTypeDef",
     "UpdateSubscriptionsToEventBridgeResponseTypeDef",
     "SubnetTypeDef",
     "BatchStartRecommendationsResponseTypeDef",
     "ImportCertificateMessageRequestTypeDef",
     "DeleteCertificateResponseTypeDef",
     "DescribeCertificatesResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "CollectorResponseTypeDef",
+    "CreateReplicationConfigMessageRequestTypeDef",
+    "ModifyReplicationConfigMessageRequestTypeDef",
+    "ReplicationConfigTypeDef",
     "DeleteConnectionResponseTypeDef",
     "DescribeConnectionsResponseTypeDef",
     "TestConnectionResponseTypeDef",
     "CreateEndpointMessageRequestTypeDef",
     "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
     "CreateEventSubscriptionResponseTypeDef",
     "DeleteEventSubscriptionResponseTypeDef",
     "DescribeEventSubscriptionsResponseTypeDef",
     "ModifyEventSubscriptionResponseTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
+    "StartReplicationMessageRequestTypeDef",
     "StartReplicationTaskMessageRequestTypeDef",
     "DatabaseResponseTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
     "DescribeEndpointsMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
@@ -200,19 +216,22 @@
     "DescribeFleetAdvisorCollectorsRequestRequestTypeDef",
     "DescribeFleetAdvisorDatabasesRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemasRequestRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "DescribeRecommendationLimitationsRequestRequestTypeDef",
     "DescribeRecommendationsRequestRequestTypeDef",
+    "DescribeReplicationConfigsMessageRequestTypeDef",
     "DescribeReplicationInstancesMessageRequestTypeDef",
     "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
+    "DescribeReplicationTableStatisticsMessageRequestTypeDef",
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
     "DescribeReplicationTasksMessageRequestTypeDef",
+    "DescribeReplicationsMessageRequestTypeDef",
     "DescribeTableStatisticsMessageRequestTypeDef",
     "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
@@ -229,45 +248,56 @@
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskStoppedWaitTypeDef",
     "DescribeEndpointSettingsResponseTypeDef",
     "DescribeEndpointTypesResponseTypeDef",
+    "DescribeEngineVersionsResponseTypeDef",
     "DescribeEventCategoriesResponseTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
     "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
     "DescribeOrderableReplicationInstancesResponseTypeDef",
     "DescribeRecommendationLimitationsResponseTypeDef",
     "DescribeRefreshSchemasStatusResponseTypeDef",
     "RefreshSchemasResponseTypeDef",
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
+    "DescribeReplicationTableStatisticsResponseTypeDef",
+    "DescribeTableStatisticsResponseTypeDef",
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
-    "DescribeTableStatisticsResponseTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "RdsRecommendationTypeDef",
     "StartRecommendationsRequestEntryTypeDef",
     "StartRecommendationsRequestRequestTypeDef",
+    "ReloadReplicationTablesMessageRequestTypeDef",
     "ReloadTablesMessageRequestTypeDef",
+    "ReplicationTypeDef",
     "ReplicationTaskAssessmentRunTypeDef",
     "ReplicationTaskTypeDef",
     "SchemaResponseTypeDef",
     "ReplicationSubnetGroupTypeDef",
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
+    "CreateReplicationConfigResponseTypeDef",
+    "DeleteReplicationConfigResponseTypeDef",
+    "DescribeReplicationConfigsResponseTypeDef",
+    "ModifyReplicationConfigResponseTypeDef",
     "CreateEndpointResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ModifyEndpointResponseTypeDef",
     "DescribeFleetAdvisorDatabasesResponseTypeDef",
     "ApplyPendingMaintenanceActionResponseTypeDef",
     "DescribePendingMaintenanceActionsResponseTypeDef",
     "RecommendationDataTypeDef",
     "BatchStartRecommendationsRequestRequestTypeDef",
+    "DescribeReplicationsResponseTypeDef",
+    "StartReplicationResponseTypeDef",
+    "StopReplicationResponseTypeDef",
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
     "StartReplicationTaskAssessmentRunResponseTypeDef",
     "CreateReplicationTaskResponseTypeDef",
     "DeleteReplicationTaskResponseTypeDef",
     "DescribeReplicationTasksResponseTypeDef",
@@ -398,14 +428,30 @@
     {
         "CollectorReferencedId": str,
         "CollectorName": str,
     },
     total=False,
 )
 
+ComputeConfigTypeDef = TypedDict(
+    "ComputeConfigTypeDef",
+    {
+        "AvailabilityZone": str,
+        "DnsNameServers": str,
+        "KmsKeyId": str,
+        "MaxCapacityUnits": int,
+        "MinCapacityUnits": int,
+        "MultiAZ": bool,
+        "PreferredMaintenanceWindow": str,
+        "ReplicationSubnetGroupId": str,
+        "VpcSecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ReplicationInstanceArn": str,
         "EndpointArn": str,
         "Status": str,
         "LastFailureMessage": str,
@@ -434,14 +480,16 @@
         "DatabaseName": str,
         "NestingLevel": NestingLevelValueType,
         "ExtractDocId": bool,
         "DocsToInvestigate": int,
         "KmsKeyId": str,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
+        "UseUpdateLookUp": bool,
+        "ReplicateShardCollections": bool,
     },
     total=False,
 )
 
 DynamoDbSettingsTypeDef = TypedDict(
     "DynamoDbSettingsTypeDef",
     {
@@ -527,14 +575,15 @@
         "SslClientKeyArn": str,
         "SslClientKeyPassword": str,
         "SslCaCertificateArn": str,
         "SaslUsername": str,
         "SaslPassword": str,
         "NoHexPrefix": bool,
         "SaslMechanism": KafkaSaslMechanismType,
+        "SslEndpointIdentificationAlgorithm": KafkaSslEndpointIdentificationAlgorithmType,
     },
     total=False,
 )
 
 KinesisSettingsTypeDef = TypedDict(
     "KinesisSettingsTypeDef",
     {
@@ -589,14 +638,16 @@
         "NestingLevel": NestingLevelValueType,
         "ExtractDocId": str,
         "DocsToInvestigate": str,
         "AuthSource": str,
         "KmsKeyId": str,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
+        "UseUpdateLookUp": bool,
+        "ReplicateShardCollections": bool,
     },
     total=False,
 )
 
 MySQLSettingsTypeDef = TypedDict(
     "MySQLSettingsTypeDef",
     {
@@ -681,14 +732,15 @@
         "UseLogminerReader": bool,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
         "SecretsManagerOracleAsmAccessRoleArn": str,
         "SecretsManagerOracleAsmSecretId": str,
         "TrimSpaceInChar": bool,
         "ConvertTimestampWithZoneToUTC": bool,
+        "OpenTransactionWindow": int,
     },
     total=False,
 )
 
 PostgreSQLSettingsTypeDef = TypedDict(
     "PostgreSQLSettingsTypeDef",
     {
@@ -708,14 +760,18 @@
         "Username": str,
         "SlotName": str,
         "PluginName": PluginNameValueType,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
         "TrimSpaceInChar": bool,
         "MapBooleanAsBoolean": bool,
+        "MapJsonbAsClob": bool,
+        "MapLongVarcharAs": LongVarcharMappingTypeType,
+        "DatabaseMode": DatabaseModeType,
+        "BabelfishDatabaseName": str,
     },
     total=False,
 )
 
 _RequiredRedisSettingsTypeDef = TypedDict(
     "_RequiredRedisSettingsTypeDef",
     {
@@ -834,14 +890,36 @@
         "Username": str,
         "SecretsManagerAccessRoleArn": str,
         "SecretsManagerSecretId": str,
     },
     total=False,
 )
 
+_RequiredTimestreamSettingsTypeDef = TypedDict(
+    "_RequiredTimestreamSettingsTypeDef",
+    {
+        "DatabaseName": str,
+        "MemoryDuration": int,
+        "MagneticDuration": int,
+    },
+)
+_OptionalTimestreamSettingsTypeDef = TypedDict(
+    "_OptionalTimestreamSettingsTypeDef",
+    {
+        "CdcInsertsAndUpdates": bool,
+        "EnableMagneticStoreWrites": bool,
+    },
+    total=False,
+)
+
+class TimestreamSettingsTypeDef(
+    _RequiredTimestreamSettingsTypeDef, _OptionalTimestreamSettingsTypeDef
+):
+    pass
+
 EventSubscriptionTypeDef = TypedDict(
     "EventSubscriptionTypeDef",
     {
         "CustomerAwsId": str,
         "CustSubscriptionId": str,
         "SnsTopicArn": str,
         "Status": str,
@@ -951,14 +1029,21 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
+DeleteReplicationConfigMessageRequestTypeDef = TypedDict(
+    "DeleteReplicationConfigMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+    },
+)
+
 DeleteReplicationInstanceMessageRequestTypeDef = TypedDict(
     "DeleteReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
 )
 
@@ -1069,14 +1154,38 @@
         "EndpointType": ReplicationEndpointTypeValueType,
         "ReplicationInstanceEngineMinimumVersion": str,
         "EngineDisplayName": str,
     },
     total=False,
 )
 
+DescribeEngineVersionsMessageRequestTypeDef = TypedDict(
+    "DescribeEngineVersionsMessageRequestTypeDef",
+    {
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+EngineVersionTypeDef = TypedDict(
+    "EngineVersionTypeDef",
+    {
+        "Version": str,
+        "Lifecycle": str,
+        "ReleaseStatus": ReleaseStatusValuesType,
+        "LaunchDate": datetime,
+        "AutoUpgradeDate": datetime,
+        "DeprecationDate": datetime,
+        "ForceUpgradeDate": datetime,
+        "AvailableUpgrades": List[str],
+    },
+    total=False,
+)
+
 EventCategoryGroupTypeDef = TypedDict(
     "EventCategoryGroupTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
     total=False,
@@ -1208,14 +1317,44 @@
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
     total=False,
 )
 
+TableStatisticsTypeDef = TypedDict(
+    "TableStatisticsTypeDef",
+    {
+        "SchemaName": str,
+        "TableName": str,
+        "Inserts": int,
+        "Deletes": int,
+        "Updates": int,
+        "Ddls": int,
+        "AppliedInserts": int,
+        "AppliedDeletes": int,
+        "AppliedUpdates": int,
+        "AppliedDdls": int,
+        "FullLoadRows": int,
+        "FullLoadCondtnlChkFailedRows": int,
+        "FullLoadErrorRows": int,
+        "FullLoadStartTime": datetime,
+        "FullLoadEndTime": datetime,
+        "FullLoadReloaded": bool,
+        "LastUpdateTime": datetime,
+        "TableState": str,
+        "ValidationPendingRecords": int,
+        "ValidationFailedRecords": int,
+        "ValidationSuspendedRecords": int,
+        "ValidationState": str,
+        "ValidationStateDetails": str,
+    },
+    total=False,
+)
+
 DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1264,44 +1403,14 @@
 )
 
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
-TableStatisticsTypeDef = TypedDict(
-    "TableStatisticsTypeDef",
-    {
-        "SchemaName": str,
-        "TableName": str,
-        "Inserts": int,
-        "Deletes": int,
-        "Updates": int,
-        "Ddls": int,
-        "AppliedInserts": int,
-        "AppliedDeletes": int,
-        "AppliedUpdates": int,
-        "AppliedDdls": int,
-        "FullLoadRows": int,
-        "FullLoadCondtnlChkFailedRows": int,
-        "FullLoadErrorRows": int,
-        "FullLoadStartTime": datetime,
-        "FullLoadEndTime": datetime,
-        "FullLoadReloaded": bool,
-        "LastUpdateTime": datetime,
-        "TableState": str,
-        "ValidationPendingRecords": int,
-        "ValidationFailedRecords": int,
-        "ValidationSuspendedRecords": int,
-        "ValidationState": str,
-        "ValidationStateDetails": str,
-    },
-    total=False,
-)
-
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
     },
     total=False,
@@ -1398,38 +1507,53 @@
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
     total=False,
 )
 
+ProvisionDataTypeDef = TypedDict(
+    "ProvisionDataTypeDef",
+    {
+        "ProvisionState": str,
+        "ProvisionedCapacityUnits": int,
+        "DateProvisioned": datetime,
+        "IsNewProvisioningAvailable": bool,
+        "DateNewProvisioningDataAvailable": datetime,
+        "ReasonForNewProvisioningData": str,
+    },
+    total=False,
+)
+
 RdsConfigurationTypeDef = TypedDict(
     "RdsConfigurationTypeDef",
     {
         "EngineEdition": str,
         "InstanceType": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageType": str,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
+        "EngineVersion": str,
     },
     total=False,
 )
 
 RdsRequirementsTypeDef = TypedDict(
     "RdsRequirementsTypeDef",
     {
         "EngineEdition": str,
         "InstanceVcpu": float,
         "InstanceMemory": float,
         "StorageSize": int,
         "StorageIops": int,
         "DeploymentOption": str,
+        "EngineVersion": str,
     },
     total=False,
 )
 
 _RequiredRebootReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredRebootReplicationInstanceMessageRequestTypeDef",
     {
@@ -1500,14 +1624,32 @@
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
     total=False,
 )
 
+ReplicationStatsTypeDef = TypedDict(
+    "ReplicationStatsTypeDef",
+    {
+        "FullLoadProgressPercent": int,
+        "ElapsedTimeMillis": int,
+        "TablesLoaded": int,
+        "TablesLoading": int,
+        "TablesQueued": int,
+        "TablesErrored": int,
+        "FreshStartDate": datetime,
+        "StartDate": datetime,
+        "StopDate": datetime,
+        "FullLoadStartDate": datetime,
+        "FullLoadFinishDate": datetime,
+    },
+    total=False,
+)
+
 ReplicationTaskAssessmentRunProgressTypeDef = TypedDict(
     "ReplicationTaskAssessmentRunProgressTypeDef",
     {
         "IndividualAssessmentCount": int,
         "IndividualAssessmentCompletedCount": int,
     },
     total=False,
@@ -1573,14 +1715,21 @@
 
 class StartReplicationTaskAssessmentRunMessageRequestTypeDef(
     _RequiredStartReplicationTaskAssessmentRunMessageRequestTypeDef,
     _OptionalStartReplicationTaskAssessmentRunMessageRequestTypeDef,
 ):
     pass
 
+StopReplicationMessageRequestTypeDef = TypedDict(
+    "StopReplicationMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+    },
+)
+
 StopReplicationTaskMessageRequestTypeDef = TypedDict(
     "StopReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
 
@@ -1747,14 +1896,22 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReloadReplicationTablesResponseTypeDef = TypedDict(
+    "ReloadReplicationTablesResponseTypeDef",
+    {
+        "ReplicationConfigArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ReloadTablesResponseTypeDef = TypedDict(
     "ReloadTablesResponseTypeDef",
     {
         "ReplicationTaskArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1856,14 +2013,87 @@
         "CreatedDate": str,
         "ModifiedDate": str,
         "InventoryData": InventoryDataTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateReplicationConfigMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateReplicationConfigMessageRequestTypeDef",
+    {
+        "ReplicationConfigIdentifier": str,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+        "ComputeConfig": ComputeConfigTypeDef,
+        "ReplicationType": MigrationTypeValueType,
+        "TableMappings": str,
+    },
+)
+_OptionalCreateReplicationConfigMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateReplicationConfigMessageRequestTypeDef",
+    {
+        "ReplicationSettings": str,
+        "SupplementalSettings": str,
+        "ResourceIdentifier": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateReplicationConfigMessageRequestTypeDef(
+    _RequiredCreateReplicationConfigMessageRequestTypeDef,
+    _OptionalCreateReplicationConfigMessageRequestTypeDef,
+):
+    pass
+
+_RequiredModifyReplicationConfigMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyReplicationConfigMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+    },
+)
+_OptionalModifyReplicationConfigMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyReplicationConfigMessageRequestTypeDef",
+    {
+        "ReplicationConfigIdentifier": str,
+        "ReplicationType": MigrationTypeValueType,
+        "TableMappings": str,
+        "ReplicationSettings": str,
+        "SupplementalSettings": str,
+        "ComputeConfig": ComputeConfigTypeDef,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+    },
+    total=False,
+)
+
+class ModifyReplicationConfigMessageRequestTypeDef(
+    _RequiredModifyReplicationConfigMessageRequestTypeDef,
+    _OptionalModifyReplicationConfigMessageRequestTypeDef,
+):
+    pass
+
+ReplicationConfigTypeDef = TypedDict(
+    "ReplicationConfigTypeDef",
+    {
+        "ReplicationConfigIdentifier": str,
+        "ReplicationConfigArn": str,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+        "ReplicationType": MigrationTypeValueType,
+        "ComputeConfig": ComputeConfigTypeDef,
+        "ReplicationSettings": str,
+        "SupplementalSettings": str,
+        "TableMappings": str,
+        "ReplicationConfigCreateTime": datetime,
+        "ReplicationConfigUpdateTime": datetime,
+    },
+    total=False,
+)
+
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1923,14 +2153,15 @@
         "SybaseSettings": SybaseSettingsTypeDef,
         "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
         "IBMDb2Settings": IBMDb2SettingsTypeDef,
         "ResourceIdentifier": str,
         "DocDbSettings": DocDbSettingsTypeDef,
         "RedisSettings": RedisSettingsTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
+        "TimestreamSettings": TimestreamSettingsTypeDef,
     },
     total=False,
 )
 
 class CreateEndpointMessageRequestTypeDef(
     _RequiredCreateEndpointMessageRequestTypeDef, _OptionalCreateEndpointMessageRequestTypeDef
 ):
@@ -1970,14 +2201,15 @@
         "OracleSettings": OracleSettingsTypeDef,
         "SybaseSettings": SybaseSettingsTypeDef,
         "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
         "IBMDb2Settings": IBMDb2SettingsTypeDef,
         "DocDbSettings": DocDbSettingsTypeDef,
         "RedisSettings": RedisSettingsTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
+        "TimestreamSettings": TimestreamSettingsTypeDef,
     },
     total=False,
 )
 
 _RequiredModifyEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointMessageRequestTypeDef",
     {
@@ -2015,14 +2247,15 @@
         "SybaseSettings": SybaseSettingsTypeDef,
         "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
         "IBMDb2Settings": IBMDb2SettingsTypeDef,
         "DocDbSettings": DocDbSettingsTypeDef,
         "RedisSettings": RedisSettingsTypeDef,
         "ExactSettings": bool,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
+        "TimestreamSettings": TimestreamSettingsTypeDef,
     },
     total=False,
 )
 
 class ModifyEndpointMessageRequestTypeDef(
     _RequiredModifyEndpointMessageRequestTypeDef, _OptionalModifyEndpointMessageRequestTypeDef
 ):
@@ -2115,14 +2348,36 @@
 
 class ModifyReplicationTaskMessageRequestTypeDef(
     _RequiredModifyReplicationTaskMessageRequestTypeDef,
     _OptionalModifyReplicationTaskMessageRequestTypeDef,
 ):
     pass
 
+_RequiredStartReplicationMessageRequestTypeDef = TypedDict(
+    "_RequiredStartReplicationMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+        "StartReplicationType": str,
+    },
+)
+_OptionalStartReplicationMessageRequestTypeDef = TypedDict(
+    "_OptionalStartReplicationMessageRequestTypeDef",
+    {
+        "CdcStartTime": TimestampTypeDef,
+        "CdcStartPosition": str,
+        "CdcStopPosition": str,
+    },
+    total=False,
+)
+
+class StartReplicationMessageRequestTypeDef(
+    _RequiredStartReplicationMessageRequestTypeDef, _OptionalStartReplicationMessageRequestTypeDef
+):
+    pass
+
 _RequiredStartReplicationTaskMessageRequestTypeDef = TypedDict(
     "_RequiredStartReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "StartReplicationTaskType": StartReplicationTaskTypeValueType,
     },
 )
@@ -2299,14 +2554,24 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeReplicationConfigsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationConfigsMessageRequestTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
 DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
     "DescribeReplicationInstancesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2319,14 +2584,36 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredDescribeReplicationTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeReplicationTableStatisticsMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+    },
+)
+_OptionalDescribeReplicationTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeReplicationTableStatisticsMessageRequestTypeDef",
+    {
+        "MaxRecords": int,
+        "Marker": str,
+        "Filters": Sequence[FilterTypeDef],
+    },
+    total=False,
+)
+
+class DescribeReplicationTableStatisticsMessageRequestTypeDef(
+    _RequiredDescribeReplicationTableStatisticsMessageRequestTypeDef,
+    _OptionalDescribeReplicationTableStatisticsMessageRequestTypeDef,
+):
+    pass
+
 DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2350,14 +2637,24 @@
         "MaxRecords": int,
         "Marker": str,
         "WithoutSettings": bool,
     },
     total=False,
 )
 
+DescribeReplicationsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationsMessageRequestTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
 _RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
 _OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
@@ -2629,14 +2926,23 @@
     {
         "Marker": str,
         "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeEngineVersionsResponseTypeDef = TypedDict(
+    "DescribeEngineVersionsResponseTypeDef",
+    {
+        "EngineVersions": List[EngineVersionTypeDef],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeEventCategoriesResponseTypeDef = TypedDict(
     "DescribeEventCategoriesResponseTypeDef",
     {
         "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2708,14 +3014,34 @@
         "ReplicationInstanceArn": str,
         "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeReplicationTableStatisticsResponseTypeDef = TypedDict(
+    "DescribeReplicationTableStatisticsResponseTypeDef",
+    {
+        "ReplicationConfigArn": str,
+        "Marker": str,
+        "ReplicationTableStatistics": List[TableStatisticsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTableStatisticsResponseTypeDef = TypedDict(
+    "DescribeTableStatisticsResponseTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "TableStatistics": List[TableStatisticsTypeDef],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     {
         "Marker": str,
         "BucketName": str,
         "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2727,24 +3053,14 @@
     {
         "Marker": str,
         "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeTableStatisticsResponseTypeDef = TypedDict(
-    "DescribeTableStatisticsResponseTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "TableStatistics": List[TableStatisticsTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -2771,14 +3087,35 @@
     "StartRecommendationsRequestRequestTypeDef",
     {
         "DatabaseId": str,
         "Settings": RecommendationSettingsTypeDef,
     },
 )
 
+_RequiredReloadReplicationTablesMessageRequestTypeDef = TypedDict(
+    "_RequiredReloadReplicationTablesMessageRequestTypeDef",
+    {
+        "ReplicationConfigArn": str,
+        "TablesToReload": Sequence[TableToReloadTypeDef],
+    },
+)
+_OptionalReloadReplicationTablesMessageRequestTypeDef = TypedDict(
+    "_OptionalReloadReplicationTablesMessageRequestTypeDef",
+    {
+        "ReloadOption": ReloadOptionValueType,
+    },
+    total=False,
+)
+
+class ReloadReplicationTablesMessageRequestTypeDef(
+    _RequiredReloadReplicationTablesMessageRequestTypeDef,
+    _OptionalReloadReplicationTablesMessageRequestTypeDef,
+):
+    pass
+
 _RequiredReloadTablesMessageRequestTypeDef = TypedDict(
     "_RequiredReloadTablesMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TablesToReload": Sequence[TableToReloadTypeDef],
     },
 )
@@ -2791,14 +3128,39 @@
 )
 
 class ReloadTablesMessageRequestTypeDef(
     _RequiredReloadTablesMessageRequestTypeDef, _OptionalReloadTablesMessageRequestTypeDef
 ):
     pass
 
+ReplicationTypeDef = TypedDict(
+    "ReplicationTypeDef",
+    {
+        "ReplicationConfigIdentifier": str,
+        "ReplicationConfigArn": str,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+        "ReplicationType": MigrationTypeValueType,
+        "Status": str,
+        "ProvisionData": ProvisionDataTypeDef,
+        "StopReason": str,
+        "FailureMessages": List[str],
+        "ReplicationStats": ReplicationStatsTypeDef,
+        "StartReplicationType": str,
+        "CdcStartTime": datetime,
+        "CdcStartPosition": str,
+        "CdcStopPosition": str,
+        "RecoveryCheckpoint": str,
+        "ReplicationCreateTime": datetime,
+        "ReplicationUpdateTime": datetime,
+        "ReplicationLastStopTime": datetime,
+    },
+    total=False,
+)
+
 ReplicationTaskAssessmentRunTypeDef = TypedDict(
     "ReplicationTaskAssessmentRunTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
         "ReplicationTaskArn": str,
         "Status": str,
         "ReplicationTaskAssessmentRunCreationDate": datetime,
@@ -2874,14 +3236,47 @@
     {
         "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateReplicationConfigResponseTypeDef = TypedDict(
+    "CreateReplicationConfigResponseTypeDef",
+    {
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteReplicationConfigResponseTypeDef = TypedDict(
+    "DeleteReplicationConfigResponseTypeDef",
+    {
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReplicationConfigsResponseTypeDef = TypedDict(
+    "DescribeReplicationConfigsResponseTypeDef",
+    {
+        "Marker": str,
+        "ReplicationConfigs": List[ReplicationConfigTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyReplicationConfigResponseTypeDef = TypedDict(
+    "ModifyReplicationConfigResponseTypeDef",
+    {
+        "ReplicationConfig": ReplicationConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2949,14 +3344,39 @@
     "BatchStartRecommendationsRequestRequestTypeDef",
     {
         "Data": Sequence[StartRecommendationsRequestEntryTypeDef],
     },
     total=False,
 )
 
+DescribeReplicationsResponseTypeDef = TypedDict(
+    "DescribeReplicationsResponseTypeDef",
+    {
+        "Marker": str,
+        "Replications": List[ReplicationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReplicationResponseTypeDef = TypedDict(
+    "StartReplicationResponseTypeDef",
+    {
+        "Replication": ReplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopReplicationResponseTypeDef = TypedDict(
+    "StopReplicationResponseTypeDef",
+    {
+        "Replication": ReplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/waiter.py` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms/waiter.pyi` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms.egg-info/PKG-INFO` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dms
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dms)](https://pepy.tech/project/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DatabaseMigrationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[aiobotocore.DatabaseMigrationService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dms-2.5.2.post3/types_aiobotocore_dms.egg-info/SOURCES.txt` & `types-aiobotocore-dms-2.5.4/types_aiobotocore_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

