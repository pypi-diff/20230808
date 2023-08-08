# Comparing `tmp/types-aiobotocore-rds-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-rds-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rds-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-rds-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
```

## Comparing `types-aiobotocore-rds-2.5.2.post1.tar` & `types-aiobotocore-rds-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:51.913485 types-aiobotocore-rds-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:25.000000 types-aiobotocore-rds-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41651 2023-08-02 14:52:51.913485 types-aiobotocore-rds-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40149 2023-08-02 14:47:25.000000 types-aiobotocore-rds-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:51.913485 types-aiobotocore-rds-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:47:25.000000 types-aiobotocore-rds-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:51.905485 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-08-02 14:47:25.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-08-02 14:47:25.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:47:25.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   148708 2023-08-02 14:47:27.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   148513 2023-08-02 14:47:26.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17798 2023-08-02 14:47:27.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-08-02 14:47:27.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    46920 2023-08-02 14:47:27.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    46883 2023-08-02 14:47:27.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:25.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   190994 2023-08-02 14:47:33.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   190817 2023-08-02 14:47:29.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:25.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-08-02 14:47:27.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-08-02 14:47:27.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:51.913485 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41651 2023-08-02 14:52:51.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:51.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:51.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:51.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:51.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:51.000000 types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.676643 types-aiobotocore-rds-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:02.000000 types-aiobotocore-rds-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20992 2023-08-04 13:59:22.676643 types-aiobotocore-rds-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19490 2023-08-04 13:50:02.000000 types-aiobotocore-rds-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.676643 types-aiobotocore-rds-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:50:01.000000 types-aiobotocore-rds-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.676643 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11394 2023-08-04 13:50:02.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11393 2023-08-04 13:50:02.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:50:02.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   151407 2023-08-04 13:50:03.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   151210 2023-08-04 13:50:03.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18059 2023-08-04 13:50:04.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18057 2023-08-04 13:50:04.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    46960 2023-08-04 13:50:04.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    46923 2023-08-04 13:50:03.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:02.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   193924 2023-08-04 13:50:12.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   193747 2023-08-04 13:50:09.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:02.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11764 2023-08-04 13:50:04.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11755 2023-08-04 13:50:04.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.676643 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20992 2023-08-04 13:59:22.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      802 2023-08-04 13:59:22.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:22.000000 types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rds-2.5.2.post1/LICENSE` & `types-aiobotocore-rds-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-2.5.2.post1/setup.py` & `types-aiobotocore-rds-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rds",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_rds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.RDS 2.5.2 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/__init__.py` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/__init__.pyi` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/__main__.py` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RDS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.RDS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post1")
+    print("2.5.2.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/client.py` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     CreateDBProxyResponseTypeDef,
     CreateDBSecurityGroupResultTypeDef,
     CreateDBSnapshotResultTypeDef,
     CreateDBSubnetGroupResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateGlobalClusterResultTypeDef,
     CreateOptionGroupResultTypeDef,
+    DBClusterAutomatedBackupMessageTypeDef,
     DBClusterBacktrackMessageTypeDef,
     DBClusterBacktrackResponseTypeDef,
     DBClusterCapacityInfoTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterEndpointResponseTypeDef,
     DBClusterMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
@@ -113,14 +114,15 @@
     DBParameterGroupDetailsTypeDef,
     DBParameterGroupNameMessageTypeDef,
     DBParameterGroupsMessageTypeDef,
     DBSecurityGroupMessageTypeDef,
     DBSnapshotMessageTypeDef,
     DBSubnetGroupMessageTypeDef,
     DeleteBlueGreenDeploymentResponseTypeDef,
+    DeleteDBClusterAutomatedBackupResultTypeDef,
     DeleteDBClusterResultTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DeleteDBInstanceAutomatedBackupResultTypeDef,
     DeleteDBInstanceResultTypeDef,
     DeleteDBProxyEndpointResponseTypeDef,
     DeleteDBProxyResponseTypeDef,
     DeleteDBSnapshotResultTypeDef,
@@ -162,15 +164,15 @@
     ModifyEventSubscriptionResultTypeDef,
     ModifyGlobalClusterResultTypeDef,
     ModifyOptionGroupResultTypeDef,
     OptionConfigurationTypeDef,
     OptionGroupOptionsMessageTypeDef,
     OptionGroupsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
-    ParameterUnionTypeDef,
+    ParameterTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
     ProcessorFeatureTypeDef,
     PromoteReadReplicaDBClusterResultTypeDef,
     PromoteReadReplicaResultTypeDef,
     PurchaseReservedDBInstancesOfferingResultTypeDef,
     RebootDBClusterResultTypeDef,
     RebootDBInstanceResultTypeDef,
@@ -244,14 +246,16 @@
     ClientError: Type[BotocoreClientError]
     CreateCustomDBEngineVersionFault: Type[BotocoreClientError]
     CustomAvailabilityZoneNotFoundFault: Type[BotocoreClientError]
     CustomDBEngineVersionAlreadyExistsFault: Type[BotocoreClientError]
     CustomDBEngineVersionNotFoundFault: Type[BotocoreClientError]
     CustomDBEngineVersionQuotaExceededFault: Type[BotocoreClientError]
     DBClusterAlreadyExistsFault: Type[BotocoreClientError]
+    DBClusterAutomatedBackupNotFoundFault: Type[BotocoreClientError]
+    DBClusterAutomatedBackupQuotaExceededFault: Type[BotocoreClientError]
     DBClusterBacktrackNotFoundFault: Type[BotocoreClientError]
     DBClusterEndpointAlreadyExistsFault: Type[BotocoreClientError]
     DBClusterEndpointNotFoundFault: Type[BotocoreClientError]
     DBClusterEndpointQuotaExceededFault: Type[BotocoreClientError]
     DBClusterNotFoundFault: Type[BotocoreClientError]
     DBClusterParameterGroupNotFoundFault: Type[BotocoreClientError]
     DBClusterQuotaExceededFault: Type[BotocoreClientError]
@@ -306,14 +310,15 @@
     InstanceQuotaExceededFault: Type[BotocoreClientError]
     InsufficientAvailableIPsInSubnetFault: Type[BotocoreClientError]
     InsufficientDBClusterCapacityFault: Type[BotocoreClientError]
     InsufficientDBInstanceCapacityFault: Type[BotocoreClientError]
     InsufficientStorageClusterCapacityFault: Type[BotocoreClientError]
     InvalidBlueGreenDeploymentStateFault: Type[BotocoreClientError]
     InvalidCustomDBEngineVersionStateFault: Type[BotocoreClientError]
+    InvalidDBClusterAutomatedBackupStateFault: Type[BotocoreClientError]
     InvalidDBClusterCapacityFault: Type[BotocoreClientError]
     InvalidDBClusterEndpointStateFault: Type[BotocoreClientError]
     InvalidDBClusterSnapshotStateFault: Type[BotocoreClientError]
     InvalidDBClusterStateFault: Type[BotocoreClientError]
     InvalidDBInstanceAutomatedBackupStateFault: Type[BotocoreClientError]
     InvalidDBInstanceStateFault: Type[BotocoreClientError]
     InvalidDBParameterGroupStateFault: Type[BotocoreClientError]
@@ -657,14 +662,15 @@
         PerformanceInsightsKMSKeyId: str = ...,
         PerformanceInsightsRetentionPeriod: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         DBSystemId: str = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
+        EnableLocalWriteForwarding: bool = ...,
         SourceRegion: str = ...
     ) -> CreateDBClusterResultTypeDef:
         """
         Creates a new Amazon Aurora DB cluster or Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_cluster)
@@ -749,14 +755,18 @@
         DBClusterIdentifier: str = ...,
         StorageType: str = ...,
         TdeCredentialArn: str = ...,
         TdeCredentialPassword: str = ...,
         StorageEncrypted: bool = ...,
         KmsKeyId: str = ...,
         Domain: str = ...,
+        DomainFqdn: str = ...,
+        DomainOu: str = ...,
+        DomainAuthSecretArn: str = ...,
+        DomainDnsIps: Sequence[str] = ...,
         CopyTagsToSnapshot: bool = ...,
         MonitoringInterval: int = ...,
         MonitoringRoleArn: str = ...,
         DomainIAMRoleName: str = ...,
         PromotionTier: int = ...,
         Timezone: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
@@ -770,15 +780,16 @@
         EnableCustomerOwnedIp: bool = ...,
         CustomIamInstanceProfile: str = ...,
         BackupTarget: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
-        CACertificateIdentifier: str = ...
+        CACertificateIdentifier: str = ...,
+        DBSystemId: str = ...
     ) -> CreateDBInstanceResultTypeDef:
         """
         Creates a new DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_instance)
         """
@@ -812,14 +823,18 @@
         PerformanceInsightsRetentionPeriod: int = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         ProcessorFeatures: Sequence[ProcessorFeatureTypeDef] = ...,
         UseDefaultProcessorFeatures: bool = ...,
         DeletionProtection: bool = ...,
         Domain: str = ...,
         DomainIAMRoleName: str = ...,
+        DomainFqdn: str = ...,
+        DomainOu: str = ...,
+        DomainAuthSecretArn: str = ...,
+        DomainDnsIps: Sequence[str] = ...,
         ReplicaMode: ReplicaModeType = ...,
         MaxAllocatedStorage: int = ...,
         CustomIamInstanceProfile: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         EnableCustomerOwnedIp: bool = ...,
         AllocatedStorage: int = ...,
@@ -1004,23 +1019,35 @@
         """
 
     async def delete_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...
+        FinalDBSnapshotIdentifier: str = ...,
+        DeleteAutomatedBackups: bool = ...
     ) -> DeleteDBClusterResultTypeDef:
         """
         The DeleteDBCluster action deletes a previously provisioned DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#delete_db_cluster)
         """
 
+    async def delete_db_cluster_automated_backup(
+        self, *, DbClusterResourceId: str
+    ) -> DeleteDBClusterAutomatedBackupResultTypeDef:
+        """
+        Deletes automated backups using the `DbClusterResourceId` value of the source DB
+        cluster or the Amazon Resource Name (ARN) of the automated backups.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster_automated_backup)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#delete_db_cluster_automated_backup)
+        """
+
     async def delete_db_cluster_endpoint(
         self, *, DBClusterEndpointIdentifier: str
     ) -> DBClusterEndpointResponseTypeDef:
         """
         Deletes a custom endpoint and removes it from an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster_endpoint)
@@ -1188,15 +1215,15 @@
         *,
         BlueGreenDeploymentIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...
     ) -> DescribeBlueGreenDeploymentsResponseTypeDef:
         """
-        Returns information about blue/green deployments.
+        Describes one or more blue/green deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_blue_green_deployments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_blue_green_deployments)
         """
 
     async def describe_certificates(
         self,
@@ -1210,14 +1237,30 @@
         Lists the set of CA certificates provided by Amazon RDS for this Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_certificates)
         """
 
+    async def describe_db_cluster_automated_backups(
+        self,
+        *,
+        DbClusterResourceId: str = ...,
+        DBClusterIdentifier: str = ...,
+        Filters: Sequence[FilterTypeDef] = ...,
+        MaxRecords: int = ...,
+        Marker: str = ...
+    ) -> DBClusterAutomatedBackupMessageTypeDef:
+        """
+        Displays backups for both current and deleted DB clusters.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_automated_backups)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_automated_backups)
+        """
+
     async def describe_db_cluster_backtracks(
         self,
         *,
         DBClusterIdentifier: str,
         BacktrackIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
@@ -1294,15 +1337,16 @@
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        IncludePublic: bool = ...
+        IncludePublic: bool = ...,
+        DbClusterResourceId: str = ...
     ) -> DBClusterSnapshotMessageTypeDef:
         """
         Returns information about DB cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_snapshots)
         """
@@ -1964,15 +2008,16 @@
         PerformanceInsightsRetentionPeriod: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         ManageMasterUserPassword: bool = ...,
         RotateMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         EngineMode: str = ...,
-        AllowEngineModeChange: bool = ...
+        AllowEngineModeChange: bool = ...,
+        EnableLocalWriteForwarding: bool = ...
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modifies the settings of an Amazon Aurora DB cluster or a Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_cluster)
         """
@@ -1989,15 +2034,15 @@
         Modifies the properties of an endpoint in an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_cluster_endpoint)
         """
 
     async def modify_db_cluster_parameter_group(
-        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
+        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_cluster_parameter_group)
         """
@@ -2042,20 +2087,25 @@
         OptionGroupName: str = ...,
         NewDBInstanceIdentifier: str = ...,
         StorageType: str = ...,
         TdeCredentialArn: str = ...,
         TdeCredentialPassword: str = ...,
         CACertificateIdentifier: str = ...,
         Domain: str = ...,
+        DomainFqdn: str = ...,
+        DomainOu: str = ...,
+        DomainAuthSecretArn: str = ...,
+        DomainDnsIps: Sequence[str] = ...,
         CopyTagsToSnapshot: bool = ...,
         MonitoringInterval: int = ...,
         DBPortNumber: int = ...,
         PubliclyAccessible: bool = ...,
         MonitoringRoleArn: str = ...,
         DomainIAMRoleName: str = ...,
+        DisableDomain: bool = ...,
         PromotionTier: int = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnablePerformanceInsights: bool = ...,
         PerformanceInsightsKMSKeyId: str = ...,
         PerformanceInsightsRetentionPeriod: int = ...,
         CloudwatchLogsExportConfiguration: CloudwatchLogsExportConfigurationTypeDef = ...,
         ProcessorFeatures: Sequence[ProcessorFeatureTypeDef] = ...,
@@ -2079,15 +2129,15 @@
         Modifies settings for a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_instance)
         """
 
     async def modify_db_parameter_group(
-        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
+        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_parameter_group)
         """
@@ -2202,15 +2252,15 @@
         GlobalClusterIdentifier: str = ...,
         NewGlobalClusterIdentifier: str = ...,
         DeletionProtection: bool = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...
     ) -> ModifyGlobalClusterResultTypeDef:
         """
-        Modify a setting for an Amazon Aurora global cluster.
+        Modifies a setting for an Amazon Aurora global cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_global_cluster)
         """
 
     async def modify_option_group(
         self,
@@ -2354,29 +2404,29 @@
         """
 
     async def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterUnionTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#reset_db_cluster_parameter_group)
         """
 
     async def reset_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterUnionTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group to the engine/system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#reset_db_parameter_group)
@@ -2469,16 +2519,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_cluster_from_snapshot)
         """
 
     async def restore_db_cluster_to_point_in_time(
         self,
         *,
         DBClusterIdentifier: str,
-        SourceDBClusterIdentifier: str,
         RestoreType: str = ...,
+        SourceDBClusterIdentifier: str = ...,
         RestoreToTime: TimestampTypeDef = ...,
         UseLatestRestorableTime: bool = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         OptionGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
@@ -2494,15 +2544,16 @@
         ScalingConfiguration: ScalingConfigurationTypeDef = ...,
         EngineMode: str = ...,
         DBClusterInstanceClass: str = ...,
         StorageType: str = ...,
         PubliclyAccessible: bool = ...,
         Iops: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
-        NetworkType: str = ...
+        NetworkType: str = ...,
+        SourceDbClusterResourceId: str = ...
     ) -> RestoreDBClusterToPointInTimeResultTypeDef:
         """
         Restores a DB cluster to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_cluster_to_point_in_time)
         """
@@ -2526,14 +2577,18 @@
         OptionGroupName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         StorageType: str = ...,
         TdeCredentialArn: str = ...,
         TdeCredentialPassword: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Domain: str = ...,
+        DomainFqdn: str = ...,
+        DomainOu: str = ...,
+        DomainAuthSecretArn: str = ...,
+        DomainDnsIps: Sequence[str] = ...,
         CopyTagsToSnapshot: bool = ...,
         DomainIAMRoleName: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         ProcessorFeatures: Sequence[ProcessorFeatureTypeDef] = ...,
         UseDefaultProcessorFeatures: bool = ...,
         DBParameterGroupName: str = ...,
@@ -2636,14 +2691,18 @@
         Tags: Sequence[TagTypeDef] = ...,
         StorageType: str = ...,
         TdeCredentialArn: str = ...,
         TdeCredentialPassword: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Domain: str = ...,
         DomainIAMRoleName: str = ...,
+        DomainFqdn: str = ...,
+        DomainOu: str = ...,
+        DomainAuthSecretArn: str = ...,
+        DomainDnsIps: Sequence[str] = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         ProcessorFeatures: Sequence[ProcessorFeatureTypeDef] = ...,
         UseDefaultProcessorFeatures: bool = ...,
         DBParameterGroupName: str = ...,
         DeletionProtection: bool = ...,
         SourceDbiResourceId: str = ...,
```

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/client.pyi` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     CreateDBProxyResponseTypeDef,
     CreateDBSecurityGroupResultTypeDef,
     CreateDBSnapshotResultTypeDef,
     CreateDBSubnetGroupResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateGlobalClusterResultTypeDef,
     CreateOptionGroupResultTypeDef,
+    DBClusterAutomatedBackupMessageTypeDef,
     DBClusterBacktrackMessageTypeDef,
     DBClusterBacktrackResponseTypeDef,
     DBClusterCapacityInfoTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterEndpointResponseTypeDef,
     DBClusterMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
@@ -113,14 +114,15 @@
     DBParameterGroupDetailsTypeDef,
     DBParameterGroupNameMessageTypeDef,
     DBParameterGroupsMessageTypeDef,
     DBSecurityGroupMessageTypeDef,
     DBSnapshotMessageTypeDef,
     DBSubnetGroupMessageTypeDef,
     DeleteBlueGreenDeploymentResponseTypeDef,
+    DeleteDBClusterAutomatedBackupResultTypeDef,
     DeleteDBClusterResultTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DeleteDBInstanceAutomatedBackupResultTypeDef,
     DeleteDBInstanceResultTypeDef,
     DeleteDBProxyEndpointResponseTypeDef,
     DeleteDBProxyResponseTypeDef,
     DeleteDBSnapshotResultTypeDef,
@@ -162,15 +164,15 @@
     ModifyEventSubscriptionResultTypeDef,
     ModifyGlobalClusterResultTypeDef,
     ModifyOptionGroupResultTypeDef,
     OptionConfigurationTypeDef,
     OptionGroupOptionsMessageTypeDef,
     OptionGroupsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
-    ParameterUnionTypeDef,
+    ParameterTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
     ProcessorFeatureTypeDef,
     PromoteReadReplicaDBClusterResultTypeDef,
     PromoteReadReplicaResultTypeDef,
     PurchaseReservedDBInstancesOfferingResultTypeDef,
     RebootDBClusterResultTypeDef,
     RebootDBInstanceResultTypeDef,
@@ -241,14 +243,16 @@
     ClientError: Type[BotocoreClientError]
     CreateCustomDBEngineVersionFault: Type[BotocoreClientError]
     CustomAvailabilityZoneNotFoundFault: Type[BotocoreClientError]
     CustomDBEngineVersionAlreadyExistsFault: Type[BotocoreClientError]
     CustomDBEngineVersionNotFoundFault: Type[BotocoreClientError]
     CustomDBEngineVersionQuotaExceededFault: Type[BotocoreClientError]
     DBClusterAlreadyExistsFault: Type[BotocoreClientError]
+    DBClusterAutomatedBackupNotFoundFault: Type[BotocoreClientError]
+    DBClusterAutomatedBackupQuotaExceededFault: Type[BotocoreClientError]
     DBClusterBacktrackNotFoundFault: Type[BotocoreClientError]
     DBClusterEndpointAlreadyExistsFault: Type[BotocoreClientError]
     DBClusterEndpointNotFoundFault: Type[BotocoreClientError]
     DBClusterEndpointQuotaExceededFault: Type[BotocoreClientError]
     DBClusterNotFoundFault: Type[BotocoreClientError]
     DBClusterParameterGroupNotFoundFault: Type[BotocoreClientError]
     DBClusterQuotaExceededFault: Type[BotocoreClientError]
@@ -303,14 +307,15 @@
     InstanceQuotaExceededFault: Type[BotocoreClientError]
     InsufficientAvailableIPsInSubnetFault: Type[BotocoreClientError]
     InsufficientDBClusterCapacityFault: Type[BotocoreClientError]
     InsufficientDBInstanceCapacityFault: Type[BotocoreClientError]
     InsufficientStorageClusterCapacityFault: Type[BotocoreClientError]
     InvalidBlueGreenDeploymentStateFault: Type[BotocoreClientError]
     InvalidCustomDBEngineVersionStateFault: Type[BotocoreClientError]
+    InvalidDBClusterAutomatedBackupStateFault: Type[BotocoreClientError]
     InvalidDBClusterCapacityFault: Type[BotocoreClientError]
     InvalidDBClusterEndpointStateFault: Type[BotocoreClientError]
     InvalidDBClusterSnapshotStateFault: Type[BotocoreClientError]
     InvalidDBClusterStateFault: Type[BotocoreClientError]
     InvalidDBInstanceAutomatedBackupStateFault: Type[BotocoreClientError]
     InvalidDBInstanceStateFault: Type[BotocoreClientError]
     InvalidDBParameterGroupStateFault: Type[BotocoreClientError]
@@ -635,14 +640,15 @@
         PerformanceInsightsKMSKeyId: str = ...,
         PerformanceInsightsRetentionPeriod: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         DBSystemId: str = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
+        EnableLocalWriteForwarding: bool = ...,
         SourceRegion: str = ...
     ) -> CreateDBClusterResultTypeDef:
         """
         Creates a new Amazon Aurora DB cluster or Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_cluster)
@@ -723,14 +729,18 @@
         DBClusterIdentifier: str = ...,
         StorageType: str = ...,
         TdeCredentialArn: str = ...,
         TdeCredentialPassword: str = ...,
         StorageEncrypted: bool = ...,
         KmsKeyId: str = ...,
         Domain: str = ...,
+        DomainFqdn: str = ...,
+        DomainOu: str = ...,
+        DomainAuthSecretArn: str = ...,
+        DomainDnsIps: Sequence[str] = ...,
         CopyTagsToSnapshot: bool = ...,
         MonitoringInterval: int = ...,
         MonitoringRoleArn: str = ...,
         DomainIAMRoleName: str = ...,
         PromotionTier: int = ...,
         Timezone: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
@@ -744,15 +754,16 @@
         EnableCustomerOwnedIp: bool = ...,
         CustomIamInstanceProfile: str = ...,
         BackupTarget: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
-        CACertificateIdentifier: str = ...
+        CACertificateIdentifier: str = ...,
+        DBSystemId: str = ...
     ) -> CreateDBInstanceResultTypeDef:
         """
         Creates a new DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#create_db_instance)
         """
@@ -785,14 +796,18 @@
         PerformanceInsightsRetentionPeriod: int = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         ProcessorFeatures: Sequence[ProcessorFeatureTypeDef] = ...,
         UseDefaultProcessorFeatures: bool = ...,
         DeletionProtection: bool = ...,
         Domain: str = ...,
         DomainIAMRoleName: str = ...,
+        DomainFqdn: str = ...,
+        DomainOu: str = ...,
+        DomainAuthSecretArn: str = ...,
+        DomainDnsIps: Sequence[str] = ...,
         ReplicaMode: ReplicaModeType = ...,
         MaxAllocatedStorage: int = ...,
         CustomIamInstanceProfile: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         EnableCustomerOwnedIp: bool = ...,
         AllocatedStorage: int = ...,
@@ -965,22 +980,33 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#delete_custom_db_engine_version)
         """
     async def delete_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...
+        FinalDBSnapshotIdentifier: str = ...,
+        DeleteAutomatedBackups: bool = ...
     ) -> DeleteDBClusterResultTypeDef:
         """
         The DeleteDBCluster action deletes a previously provisioned DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#delete_db_cluster)
         """
+    async def delete_db_cluster_automated_backup(
+        self, *, DbClusterResourceId: str
+    ) -> DeleteDBClusterAutomatedBackupResultTypeDef:
+        """
+        Deletes automated backups using the `DbClusterResourceId` value of the source DB
+        cluster or the Amazon Resource Name (ARN) of the automated backups.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster_automated_backup)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#delete_db_cluster_automated_backup)
+        """
     async def delete_db_cluster_endpoint(
         self, *, DBClusterEndpointIdentifier: str
     ) -> DBClusterEndpointResponseTypeDef:
         """
         Deletes a custom endpoint and removes it from an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_cluster_endpoint)
@@ -1132,15 +1158,15 @@
         *,
         BlueGreenDeploymentIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...
     ) -> DescribeBlueGreenDeploymentsResponseTypeDef:
         """
-        Returns information about blue/green deployments.
+        Describes one or more blue/green deployments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_blue_green_deployments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_blue_green_deployments)
         """
     async def describe_certificates(
         self,
         *,
@@ -1152,14 +1178,29 @@
         """
         Lists the set of CA certificates provided by Amazon RDS for this Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_certificates)
         """
+    async def describe_db_cluster_automated_backups(
+        self,
+        *,
+        DbClusterResourceId: str = ...,
+        DBClusterIdentifier: str = ...,
+        Filters: Sequence[FilterTypeDef] = ...,
+        MaxRecords: int = ...,
+        Marker: str = ...
+    ) -> DBClusterAutomatedBackupMessageTypeDef:
+        """
+        Displays backups for both current and deleted DB clusters.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_automated_backups)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_automated_backups)
+        """
     async def describe_db_cluster_backtracks(
         self,
         *,
         DBClusterIdentifier: str,
         BacktrackIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
@@ -1231,15 +1272,16 @@
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        IncludePublic: bool = ...
+        IncludePublic: bool = ...,
+        DbClusterResourceId: str = ...
     ) -> DBClusterSnapshotMessageTypeDef:
         """
         Returns information about DB cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.describe_db_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#describe_db_cluster_snapshots)
         """
@@ -1860,15 +1902,16 @@
         PerformanceInsightsRetentionPeriod: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
         NetworkType: str = ...,
         ManageMasterUserPassword: bool = ...,
         RotateMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         EngineMode: str = ...,
-        AllowEngineModeChange: bool = ...
+        AllowEngineModeChange: bool = ...,
+        EnableLocalWriteForwarding: bool = ...
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modifies the settings of an Amazon Aurora DB cluster or a Multi-AZ DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_cluster)
         """
@@ -1883,15 +1926,15 @@
         """
         Modifies the properties of an endpoint in an Amazon Aurora DB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_cluster_endpoint)
         """
     async def modify_db_cluster_parameter_group(
-        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
+        self, *, DBClusterParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_cluster_parameter_group)
         """
@@ -1934,20 +1977,25 @@
         OptionGroupName: str = ...,
         NewDBInstanceIdentifier: str = ...,
         StorageType: str = ...,
         TdeCredentialArn: str = ...,
         TdeCredentialPassword: str = ...,
         CACertificateIdentifier: str = ...,
         Domain: str = ...,
+        DomainFqdn: str = ...,
+        DomainOu: str = ...,
+        DomainAuthSecretArn: str = ...,
+        DomainDnsIps: Sequence[str] = ...,
         CopyTagsToSnapshot: bool = ...,
         MonitoringInterval: int = ...,
         DBPortNumber: int = ...,
         PubliclyAccessible: bool = ...,
         MonitoringRoleArn: str = ...,
         DomainIAMRoleName: str = ...,
+        DisableDomain: bool = ...,
         PromotionTier: int = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnablePerformanceInsights: bool = ...,
         PerformanceInsightsKMSKeyId: str = ...,
         PerformanceInsightsRetentionPeriod: int = ...,
         CloudwatchLogsExportConfiguration: CloudwatchLogsExportConfigurationTypeDef = ...,
         ProcessorFeatures: Sequence[ProcessorFeatureTypeDef] = ...,
@@ -1970,15 +2018,15 @@
         """
         Modifies settings for a DB instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_instance)
         """
     async def modify_db_parameter_group(
-        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterUnionTypeDef]
+        self, *, DBParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_db_parameter_group)
         """
@@ -2085,15 +2133,15 @@
         GlobalClusterIdentifier: str = ...,
         NewGlobalClusterIdentifier: str = ...,
         DeletionProtection: bool = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...
     ) -> ModifyGlobalClusterResultTypeDef:
         """
-        Modify a setting for an Amazon Aurora global cluster.
+        Modifies a setting for an Amazon Aurora global cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.modify_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#modify_global_cluster)
         """
     async def modify_option_group(
         self,
         *,
@@ -2224,28 +2272,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#remove_tags_from_resource)
         """
     async def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterUnionTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#reset_db_cluster_parameter_group)
         """
     async def reset_db_parameter_group(
         self,
         *,
         DBParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterUnionTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...
     ) -> DBParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a DB parameter group to the engine/system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.reset_db_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#reset_db_parameter_group)
@@ -2335,16 +2383,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_cluster_from_snapshot)
         """
     async def restore_db_cluster_to_point_in_time(
         self,
         *,
         DBClusterIdentifier: str,
-        SourceDBClusterIdentifier: str,
         RestoreType: str = ...,
+        SourceDBClusterIdentifier: str = ...,
         RestoreToTime: TimestampTypeDef = ...,
         UseLatestRestorableTime: bool = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         OptionGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
@@ -2360,15 +2408,16 @@
         ScalingConfiguration: ScalingConfigurationTypeDef = ...,
         EngineMode: str = ...,
         DBClusterInstanceClass: str = ...,
         StorageType: str = ...,
         PubliclyAccessible: bool = ...,
         Iops: int = ...,
         ServerlessV2ScalingConfiguration: ServerlessV2ScalingConfigurationTypeDef = ...,
-        NetworkType: str = ...
+        NetworkType: str = ...,
+        SourceDbClusterResourceId: str = ...
     ) -> RestoreDBClusterToPointInTimeResultTypeDef:
         """
         Restores a DB cluster to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_cluster_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/client/#restore_db_cluster_to_point_in_time)
         """
@@ -2391,14 +2440,18 @@
         OptionGroupName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         StorageType: str = ...,
         TdeCredentialArn: str = ...,
         TdeCredentialPassword: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Domain: str = ...,
+        DomainFqdn: str = ...,
+        DomainOu: str = ...,
+        DomainAuthSecretArn: str = ...,
+        DomainDnsIps: Sequence[str] = ...,
         CopyTagsToSnapshot: bool = ...,
         DomainIAMRoleName: str = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         ProcessorFeatures: Sequence[ProcessorFeatureTypeDef] = ...,
         UseDefaultProcessorFeatures: bool = ...,
         DBParameterGroupName: str = ...,
@@ -2499,14 +2552,18 @@
         Tags: Sequence[TagTypeDef] = ...,
         StorageType: str = ...,
         TdeCredentialArn: str = ...,
         TdeCredentialPassword: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Domain: str = ...,
         DomainIAMRoleName: str = ...,
+        DomainFqdn: str = ...,
+        DomainOu: str = ...,
+        DomainAuthSecretArn: str = ...,
+        DomainDnsIps: Sequence[str] = ...,
         EnableIAMDatabaseAuthentication: bool = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         ProcessorFeatures: Sequence[ProcessorFeatureTypeDef] = ...,
         UseDefaultProcessorFeatures: bool = ...,
         DBParameterGroupName: str = ...,
         DeletionProtection: bool = ...,
         SourceDbiResourceId: str = ...,
```

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/literals.py` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActivityStreamModeType",
     "ActivityStreamPolicyStatusType",
     "ActivityStreamStatusType",
     "ApplyMethodType",
     "AuditPolicyStateType",
     "AuthSchemeType",
@@ -76,14 +75,15 @@
     "DescribeReservedDBInstancesPaginatorName",
     "DescribeSourceRegionsPaginatorName",
     "DownloadDBLogFilePortionPaginatorName",
     "EngineFamilyType",
     "ExportSourceTypeType",
     "FailoverStatusType",
     "IAMAuthModeType",
+    "LocalWriteForwardingStatusType",
     "ReplicaModeType",
     "SourceTypeType",
     "TargetHealthReasonType",
     "TargetRoleType",
     "TargetStateType",
     "TargetTypeType",
     "WriteForwardingStatusType",
@@ -91,15 +91,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActivityStreamModeType = Literal["async", "sync"]
 ActivityStreamPolicyStatusType = Literal["locked", "locking-policy", "unlocked", "unlocking-policy"]
 ActivityStreamStatusType = Literal["started", "starting", "stopped", "stopping"]
 ApplyMethodType = Literal["immediate", "pending-reboot"]
 AuditPolicyStateType = Literal["locked", "unlocked"]
 AuthSchemeType = Literal["SECRETS"]
 AutomationModeType = Literal["all-paused", "full"]
@@ -175,14 +174,17 @@
 DescribeReservedDBInstancesPaginatorName = Literal["describe_reserved_db_instances"]
 DescribeSourceRegionsPaginatorName = Literal["describe_source_regions"]
 DownloadDBLogFilePortionPaginatorName = Literal["download_db_log_file_portion"]
 EngineFamilyType = Literal["MYSQL", "POSTGRESQL", "SQLSERVER"]
 ExportSourceTypeType = Literal["CLUSTER", "SNAPSHOT"]
 FailoverStatusType = Literal["cancelling", "failing-over", "pending"]
 IAMAuthModeType = Literal["DISABLED", "ENABLED", "REQUIRED"]
+LocalWriteForwardingStatusType = Literal[
+    "disabled", "disabling", "enabled", "enabling", "requested"
+]
 ReplicaModeType = Literal["mounted", "open-read-only"]
 SourceTypeType = Literal[
     "blue-green-deployment",
     "custom-engine-version",
     "db-cluster",
     "db-cluster-snapshot",
     "db-instance",
@@ -214,14 +216,15 @@
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
@@ -317,14 +320,15 @@
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
@@ -403,26 +407,28 @@
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
@@ -631,14 +637,15 @@
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

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/literals.pyi` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActivityStreamModeType",
     "ActivityStreamPolicyStatusType",
     "ActivityStreamStatusType",
     "ApplyMethodType",
     "AuditPolicyStateType",
     "AuthSchemeType",
@@ -75,14 +76,15 @@
     "DescribeReservedDBInstancesPaginatorName",
     "DescribeSourceRegionsPaginatorName",
     "DownloadDBLogFilePortionPaginatorName",
     "EngineFamilyType",
     "ExportSourceTypeType",
     "FailoverStatusType",
     "IAMAuthModeType",
+    "LocalWriteForwardingStatusType",
     "ReplicaModeType",
     "SourceTypeType",
     "TargetHealthReasonType",
     "TargetRoleType",
     "TargetStateType",
     "TargetTypeType",
     "WriteForwardingStatusType",
@@ -90,14 +92,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 ActivityStreamModeType = Literal["async", "sync"]
 ActivityStreamPolicyStatusType = Literal["locked", "locking-policy", "unlocked", "unlocking-policy"]
 ActivityStreamStatusType = Literal["started", "starting", "stopped", "stopping"]
 ApplyMethodType = Literal["immediate", "pending-reboot"]
 AuditPolicyStateType = Literal["locked", "unlocked"]
 AuthSchemeType = Literal["SECRETS"]
 AutomationModeType = Literal["all-paused", "full"]
@@ -173,14 +176,17 @@
 DescribeReservedDBInstancesPaginatorName = Literal["describe_reserved_db_instances"]
 DescribeSourceRegionsPaginatorName = Literal["describe_source_regions"]
 DownloadDBLogFilePortionPaginatorName = Literal["download_db_log_file_portion"]
 EngineFamilyType = Literal["MYSQL", "POSTGRESQL", "SQLSERVER"]
 ExportSourceTypeType = Literal["CLUSTER", "SNAPSHOT"]
 FailoverStatusType = Literal["cancelling", "failing-over", "pending"]
 IAMAuthModeType = Literal["DISABLED", "ENABLED", "REQUIRED"]
+LocalWriteForwardingStatusType = Literal[
+    "disabled", "disabling", "enabled", "enabling", "requested"
+]
 ReplicaModeType = Literal["mounted", "open-read-only"]
 SourceTypeType = Literal[
     "blue-green-deployment",
     "custom-engine-version",
     "db-cluster",
     "db-cluster-snapshot",
     "db-instance",
@@ -212,14 +218,15 @@
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
@@ -315,14 +322,15 @@
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
@@ -401,26 +409,28 @@
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
@@ -629,14 +639,15 @@
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

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/paginator.py` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,14 +312,15 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
+        DbClusterResourceId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclustersnapshotspaginator)
         """
```

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/paginator.pyi` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -303,14 +303,15 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
+        DbClusterResourceId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/paginators/#describedbclustersnapshotspaginator)
         """
```

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/type_defs.py` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     DBProxyEndpointStatusType,
     DBProxyEndpointTargetRoleType,
     DBProxyStatusType,
     EngineFamilyType,
     ExportSourceTypeType,
     FailoverStatusType,
     IAMAuthModeType,
+    LocalWriteForwardingStatusType,
     ReplicaModeType,
     SourceTypeType,
     TargetHealthReasonType,
     TargetRoleType,
     TargetStateType,
     TargetTypeType,
     WriteForwardingStatusType,
@@ -45,15 +46,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountQuotaTypeDef",
     "ResponseMetadataTypeDef",
     "AddRoleToDBClusterMessageRequestTypeDef",
     "AddRoleToDBInstanceMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
@@ -79,43 +79,44 @@
     "ScalingConfigurationTypeDef",
     "ServerlessV2ScalingConfigurationTypeDef",
     "ProcessorFeatureTypeDef",
     "DBProxyEndpointTypeDef",
     "UserAuthConfigTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "CustomDBEngineVersionAMITypeDef",
+    "RestoreWindowTypeDef",
     "DBClusterBacktrackTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
-    "ParameterOutputTypeDef",
+    "ParameterTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "DomainMembershipTypeDef",
     "MasterUserSecretTypeDef",
     "ScalingConfigurationInfoTypeDef",
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "TimezoneTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceAutomatedBackupsReplicationTypeDef",
-    "RestoreWindowTypeDef",
     "DBInstanceRoleTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "DBParameterGroupStatusTypeDef",
     "DBSecurityGroupMembershipTypeDef",
     "EndpointTypeDef",
     "OptionGroupMembershipTypeDef",
     "TargetHealthTypeDef",
     "UserAuthConfigInfoTypeDef",
     "EC2SecurityGroupTypeDef",
     "IPRangeTypeDef",
     "DBSnapshotAttributeTypeDef",
     "DeleteBlueGreenDeploymentRequestRequestTypeDef",
     "DeleteCustomDBEngineVersionMessageRequestTypeDef",
+    "DeleteDBClusterAutomatedBackupMessageRequestTypeDef",
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceAutomatedBackupMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBParameterGroupMessageRequestTypeDef",
@@ -156,15 +157,14 @@
     "ModifyDBSnapshotMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "OptionSettingTypeDef",
     "OptionVersionTypeDef",
     "OutpostTypeDef",
-    "ParameterTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "PromoteReadReplicaMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBClusterMessageRequestTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RecurringChargeTypeDef",
@@ -255,29 +255,35 @@
     "RestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     "CreateDBProxyEndpointResponseTypeDef",
     "DeleteDBProxyEndpointResponseTypeDef",
     "DescribeDBProxyEndpointsResponseTypeDef",
     "ModifyDBProxyEndpointResponseTypeDef",
     "CreateDBProxyRequestRequestTypeDef",
     "ModifyDBProxyRequestRequestTypeDef",
+    "DBClusterAutomatedBackupTypeDef",
     "DBClusterBacktrackMessageTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionResponseTypeDef",
     "DBEngineVersionTypeDef",
     "DBInstanceAutomatedBackupTypeDef",
     "DBProxyTargetTypeDef",
     "DBProxyTypeDef",
     "DBSecurityGroupTypeDef",
     "DBSnapshotAttributesResultTypeDef",
     "DescribeBlueGreenDeploymentsRequestRequestTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
+    "DescribeDBClusterAutomatedBackupsMessageRequestTypeDef",
     "DescribeDBClusterBacktracksMessageRequestTypeDef",
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
@@ -357,15 +363,14 @@
     "EventsMessageTypeDef",
     "ExportTasksMessageTypeDef",
     "GlobalClusterTypeDef",
     "OptionGroupOptionSettingTypeDef",
     "OptionConfigurationTypeDef",
     "OptionTypeDef",
     "SubnetTypeDef",
-    "ParameterUnionTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
     "ReservedDBInstanceTypeDef",
     "ReservedDBInstancesOfferingTypeDef",
     "SourceRegionMessageTypeDef",
     "CopyDBClusterSnapshotResultTypeDef",
     "CreateDBClusterSnapshotResultTypeDef",
@@ -380,14 +385,16 @@
     "DescribeDBProxyTargetGroupsResponseTypeDef",
     "ModifyDBProxyTargetGroupResponseTypeDef",
     "CopyDBSnapshotResultTypeDef",
     "CreateDBSnapshotResultTypeDef",
     "DBSnapshotMessageTypeDef",
     "DeleteDBSnapshotResultTypeDef",
     "ModifyDBSnapshotResultTypeDef",
+    "DBClusterAutomatedBackupMessageTypeDef",
+    "DeleteDBClusterAutomatedBackupResultTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     "DBEngineVersionMessageTypeDef",
     "DBInstanceAutomatedBackupMessageTypeDef",
     "DeleteDBInstanceAutomatedBackupResultTypeDef",
@@ -411,18 +418,14 @@
     "GlobalClustersMessageTypeDef",
     "ModifyGlobalClusterResultTypeDef",
     "RemoveFromGlobalClusterResultTypeDef",
     "OptionGroupOptionTypeDef",
     "ModifyOptionGroupMessageRequestTypeDef",
     "OptionGroupTypeDef",
     "DBSubnetGroupTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBParameterGroupMessageRequestTypeDef",
     "ApplyPendingMaintenanceActionResultTypeDef",
     "PendingMaintenanceActionsMessageTypeDef",
     "ValidDBInstanceModificationsMessageTypeDef",
     "PurchaseReservedDBInstancesOfferingResultTypeDef",
     "ReservedDBInstanceMessageTypeDef",
     "ReservedDBInstancesOfferingMessageTypeDef",
     "CreateDBClusterResultTypeDef",
@@ -494,22 +497,20 @@
     "_OptionalAddRoleToDBClusterMessageRequestTypeDef",
     {
         "FeatureName": str,
     },
     total=False,
 )
 
-
 class AddRoleToDBClusterMessageRequestTypeDef(
     _RequiredAddRoleToDBClusterMessageRequestTypeDef,
     _OptionalAddRoleToDBClusterMessageRequestTypeDef,
 ):
     pass
 
-
 AddRoleToDBInstanceMessageRequestTypeDef = TypedDict(
     "AddRoleToDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "RoleArn": str,
         "FeatureName": str,
     },
@@ -571,22 +572,20 @@
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupId": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
-
 class AuthorizeDBSecurityGroupIngressMessageRequestTypeDef(
     _RequiredAuthorizeDBSecurityGroupIngressMessageRequestTypeDef,
     _OptionalAuthorizeDBSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
-
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -673,22 +672,20 @@
     "_OptionalClientGenerateDbAuthTokenRequestTypeDef",
     {
         "Region": Optional[str],
     },
     total=False,
 )
 
-
 class ClientGenerateDbAuthTokenRequestTypeDef(
     _RequiredClientGenerateDbAuthTokenRequestTypeDef,
     _OptionalClientGenerateDbAuthTokenRequestTypeDef,
 ):
     pass
 
-
 CloudwatchLogsExportConfigurationTypeDef = TypedDict(
     "CloudwatchLogsExportConfigurationTypeDef",
     {
         "EnableLogTypes": Sequence[str],
         "DisableLogTypes": Sequence[str],
     },
     total=False,
@@ -830,14 +827,23 @@
     {
         "ImageId": str,
         "Status": str,
     },
     total=False,
 )
 
+RestoreWindowTypeDef = TypedDict(
+    "RestoreWindowTypeDef",
+    {
+        "EarliestTime": datetime,
+        "LatestTime": datetime,
+    },
+    total=False,
+)
+
 DBClusterBacktrackTypeDef = TypedDict(
     "DBClusterBacktrackTypeDef",
     {
         "DBClusterIdentifier": str,
         "BacktrackIdentifier": str,
         "BacktrackTo": datetime,
         "BacktrackedFrom": datetime,
@@ -880,16 +886,16 @@
     {
         "DBClusterOptionGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "ApplyType": str,
         "DataType": str,
@@ -924,14 +930,17 @@
 DomainMembershipTypeDef = TypedDict(
     "DomainMembershipTypeDef",
     {
         "Domain": str,
         "Status": str,
         "FQDN": str,
         "IAMRoleName": str,
+        "OU": str,
+        "AuthSecretArn": str,
+        "DnsIps": List[str],
     },
     total=False,
 )
 
 MasterUserSecretTypeDef = TypedDict(
     "MasterUserSecretTypeDef",
     {
@@ -989,35 +998,27 @@
         "Description": str,
         "AutoUpgrade": bool,
         "IsMajorVersionUpgrade": bool,
         "SupportedEngineModes": List[str],
         "SupportsParallelQuery": bool,
         "SupportsGlobalDatabases": bool,
         "SupportsBabelfish": bool,
+        "SupportsLocalWriteForwarding": bool,
     },
     total=False,
 )
 
 DBInstanceAutomatedBackupsReplicationTypeDef = TypedDict(
     "DBInstanceAutomatedBackupsReplicationTypeDef",
     {
         "DBInstanceAutomatedBackupsArn": str,
     },
     total=False,
 )
 
-RestoreWindowTypeDef = TypedDict(
-    "RestoreWindowTypeDef",
-    {
-        "EarliestTime": datetime,
-        "LatestTime": datetime,
-    },
-    total=False,
-)
-
 DBInstanceRoleTypeDef = TypedDict(
     "DBInstanceRoleTypeDef",
     {
         "RoleArn": str,
         "FeatureName": str,
         "Status": str,
     },
@@ -1134,30 +1135,35 @@
     "_OptionalDeleteBlueGreenDeploymentRequestRequestTypeDef",
     {
         "DeleteTarget": bool,
     },
     total=False,
 )
 
-
 class DeleteBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredDeleteBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalDeleteBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "DeleteCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
 
+DeleteDBClusterAutomatedBackupMessageRequestTypeDef = TypedDict(
+    "DeleteDBClusterAutomatedBackupMessageRequestTypeDef",
+    {
+        "DbClusterResourceId": str,
+    },
+)
+
 DeleteDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 
@@ -1168,25 +1174,24 @@
     },
 )
 _OptionalDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_OptionalDeleteDBClusterMessageRequestTypeDef",
     {
         "SkipFinalSnapshot": bool,
         "FinalDBSnapshotIdentifier": str,
+        "DeleteAutomatedBackups": bool,
     },
     total=False,
 )
 
-
 class DeleteDBClusterMessageRequestTypeDef(
     _RequiredDeleteDBClusterMessageRequestTypeDef, _OptionalDeleteDBClusterMessageRequestTypeDef
 ):
     pass
 
-
 DeleteDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 
@@ -1218,21 +1223,19 @@
         "SkipFinalSnapshot": bool,
         "FinalDBSnapshotIdentifier": str,
         "DeleteAutomatedBackups": bool,
     },
     total=False,
 )
 
-
 class DeleteDBInstanceMessageRequestTypeDef(
     _RequiredDeleteDBInstanceMessageRequestTypeDef, _OptionalDeleteDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 DeleteDBParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteDBParameterGroupMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
     },
 )
 
@@ -1304,22 +1307,20 @@
         "TargetGroupName": str,
         "DBInstanceIdentifiers": Sequence[str],
         "DBClusterIdentifiers": Sequence[str],
     },
     total=False,
 )
 
-
 class DeregisterDBProxyTargetsRequestRequestTypeDef(
     _RequiredDeregisterDBProxyTargetsRequestRequestTypeDef,
     _OptionalDeregisterDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
@@ -1395,22 +1396,20 @@
     {
         "Marker": str,
         "NumberOfLines": int,
     },
     total=False,
 )
 
-
 class DownloadDBLogFilePortionMessageRequestTypeDef(
     _RequiredDownloadDBLogFilePortionMessageRequestTypeDef,
     _OptionalDownloadDBLogFilePortionMessageRequestTypeDef,
 ):
     pass
 
-
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
     total=False,
@@ -1462,21 +1461,19 @@
     "_OptionalFailoverDBClusterMessageRequestTypeDef",
     {
         "TargetDBInstanceIdentifier": str,
     },
     total=False,
 )
 
-
 class FailoverDBClusterMessageRequestTypeDef(
     _RequiredFailoverDBClusterMessageRequestTypeDef, _OptionalFailoverDBClusterMessageRequestTypeDef
 ):
     pass
 
-
 FailoverGlobalClusterMessageRequestTypeDef = TypedDict(
     "FailoverGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "TargetDbClusterIdentifier": str,
     },
 )
@@ -1541,22 +1538,20 @@
         "Capacity": int,
         "SecondsBeforeTimeout": int,
         "TimeoutAction": str,
     },
     total=False,
 )
 
-
 class ModifyCurrentDBClusterCapacityMessageRequestTypeDef(
     _RequiredModifyCurrentDBClusterCapacityMessageRequestTypeDef,
     _OptionalModifyCurrentDBClusterCapacityMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
@@ -1565,22 +1560,20 @@
     {
         "Description": str,
         "Status": CustomEngineVersionStatusType,
     },
     total=False,
 )
 
-
 class ModifyCustomDBEngineVersionMessageRequestTypeDef(
     _RequiredModifyCustomDBEngineVersionMessageRequestTypeDef,
     _OptionalModifyCustomDBEngineVersionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 _OptionalModifyDBClusterEndpointMessageRequestTypeDef = TypedDict(
@@ -1589,22 +1582,20 @@
         "EndpointType": str,
         "StaticMembers": Sequence[str],
         "ExcludedMembers": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyDBClusterEndpointMessageRequestTypeDef(
     _RequiredModifyDBClusterEndpointMessageRequestTypeDef,
     _OptionalModifyDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -1613,22 +1604,20 @@
     {
         "ValuesToAdd": Sequence[str],
         "ValuesToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyDBClusterSnapshotAttributeMessageRequestTypeDef(
     _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     _OptionalModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyDBProxyEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDBProxyEndpointRequestRequestTypeDef",
     {
         "DBProxyEndpointName": str,
     },
 )
 _OptionalModifyDBProxyEndpointRequestRequestTypeDef = TypedDict(
@@ -1636,22 +1625,20 @@
     {
         "NewDBProxyEndpointName": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyDBProxyEndpointRequestRequestTypeDef(
     _RequiredModifyDBProxyEndpointRequestRequestTypeDef,
     _OptionalModifyDBProxyEndpointRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyDBSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSnapshotAttributeMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -1660,22 +1647,20 @@
     {
         "ValuesToAdd": Sequence[str],
         "ValuesToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyDBSnapshotAttributeMessageRequestTypeDef(
     _RequiredModifyDBSnapshotAttributeMessageRequestTypeDef,
     _OptionalModifyDBSnapshotAttributeMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSnapshotMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
     },
 )
 _OptionalModifyDBSnapshotMessageRequestTypeDef = TypedDict(
@@ -1683,21 +1668,19 @@
     {
         "EngineVersion": str,
         "OptionGroupName": str,
     },
     total=False,
 )
 
-
 class ModifyDBSnapshotMessageRequestTypeDef(
     _RequiredModifyDBSnapshotMessageRequestTypeDef, _OptionalModifyDBSnapshotMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -1705,22 +1688,20 @@
     "_OptionalModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupDescription": str,
     },
     total=False,
 )
 
-
 class ModifyDBSubnetGroupMessageRequestTypeDef(
     _RequiredModifyDBSubnetGroupMessageRequestTypeDef,
     _OptionalModifyDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
     },
 )
 _OptionalModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
@@ -1730,22 +1711,20 @@
         "SourceType": str,
         "EventCategories": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class ModifyEventSubscriptionMessageRequestTypeDef(
     _RequiredModifyEventSubscriptionMessageRequestTypeDef,
     _OptionalModifyEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
-
 ModifyGlobalClusterMessageRequestTypeDef = TypedDict(
     "ModifyGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "NewGlobalClusterIdentifier": str,
         "DeletionProtection": bool,
         "EngineVersion": str,
@@ -1783,32 +1762,14 @@
     "OutpostTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterValue": str,
-        "Description": str,
-        "Source": str,
-        "ApplyType": str,
-        "DataType": str,
-        "AllowedValues": str,
-        "IsModifiable": bool,
-        "MinimumEngineVersion": str,
-        "ApplyMethod": ApplyMethodType,
-        "SupportedEngineModes": Sequence[str],
-    },
-    total=False,
-)
-
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
@@ -1836,22 +1797,20 @@
     {
         "BackupRetentionPeriod": int,
         "PreferredBackupWindow": str,
     },
     total=False,
 )
 
-
 class PromoteReadReplicaMessageRequestTypeDef(
     _RequiredPromoteReadReplicaMessageRequestTypeDef,
     _OptionalPromoteReadReplicaMessageRequestTypeDef,
 ):
     pass
 
-
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "From": int,
         "To": int,
         "Step": int,
     },
@@ -1875,21 +1834,19 @@
     "_OptionalRebootDBInstanceMessageRequestTypeDef",
     {
         "ForceFailover": bool,
     },
     total=False,
 )
 
-
 class RebootDBInstanceMessageRequestTypeDef(
     _RequiredRebootDBInstanceMessageRequestTypeDef, _OptionalRebootDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
     total=False,
@@ -1907,22 +1864,20 @@
         "TargetGroupName": str,
         "DBInstanceIdentifiers": Sequence[str],
         "DBClusterIdentifiers": Sequence[str],
     },
     total=False,
 )
 
-
 class RegisterDBProxyTargetsRequestRequestTypeDef(
     _RequiredRegisterDBProxyTargetsRequestRequestTypeDef,
     _OptionalRegisterDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 RemoveFromGlobalClusterMessageRequestTypeDef = TypedDict(
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "DbClusterIdentifier": str,
     },
     total=False,
@@ -1939,22 +1894,20 @@
     "_OptionalRemoveRoleFromDBClusterMessageRequestTypeDef",
     {
         "FeatureName": str,
     },
     total=False,
 )
 
-
 class RemoveRoleFromDBClusterMessageRequestTypeDef(
     _RequiredRemoveRoleFromDBClusterMessageRequestTypeDef,
     _OptionalRemoveRoleFromDBClusterMessageRequestTypeDef,
 ):
     pass
 
-
 RemoveRoleFromDBInstanceMessageRequestTypeDef = TypedDict(
     "RemoveRoleFromDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "RoleArn": str,
         "FeatureName": str,
     },
@@ -1989,22 +1942,20 @@
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupId": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
-
 class RevokeDBSecurityGroupIngressMessageRequestTypeDef(
     _RequiredRevokeDBSecurityGroupIngressMessageRequestTypeDef,
     _OptionalRevokeDBSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
-
 SourceRegionTypeDef = TypedDict(
     "SourceRegionTypeDef",
     {
         "RegionName": str,
         "Endpoint": str,
         "Status": str,
         "SupportsDBInstanceAutomatedBackupsReplication": bool,
@@ -2025,22 +1976,20 @@
     {
         "ApplyImmediately": bool,
         "EngineNativeAuditFieldsIncluded": bool,
     },
     total=False,
 )
 
-
 class StartActivityStreamRequestRequestTypeDef(
     _RequiredStartActivityStreamRequestRequestTypeDef,
     _OptionalStartActivityStreamRequestRequestTypeDef,
 ):
     pass
 
-
 StartDBClusterMessageRequestTypeDef = TypedDict(
     "StartDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -2057,22 +2006,20 @@
         "KmsKeyId": str,
         "PreSignedUrl": str,
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class StartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef(
     _RequiredStartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef,
     _OptionalStartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef,
 ):
     pass
 
-
 StartDBInstanceMessageRequestTypeDef = TypedDict(
     "StartDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 
@@ -2091,43 +2038,39 @@
     {
         "S3Prefix": str,
         "ExportOnly": Sequence[str],
     },
     total=False,
 )
 
-
 class StartExportTaskMessageRequestTypeDef(
     _RequiredStartExportTaskMessageRequestTypeDef, _OptionalStartExportTaskMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredStopActivityStreamRequestRequestTypeDef = TypedDict(
     "_RequiredStopActivityStreamRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalStopActivityStreamRequestRequestTypeDef = TypedDict(
     "_OptionalStopActivityStreamRequestRequestTypeDef",
     {
         "ApplyImmediately": bool,
     },
     total=False,
 )
 
-
 class StopActivityStreamRequestRequestTypeDef(
     _RequiredStopActivityStreamRequestRequestTypeDef,
     _OptionalStopActivityStreamRequestRequestTypeDef,
 ):
     pass
 
-
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -2148,43 +2091,39 @@
     "_OptionalStopDBInstanceMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
     },
     total=False,
 )
 
-
 class StopDBInstanceMessageRequestTypeDef(
     _RequiredStopDBInstanceMessageRequestTypeDef, _OptionalStopDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
     },
 )
 _OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef",
     {
         "SwitchoverTimeout": int,
     },
     total=False,
 )
 
-
 class SwitchoverBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 SwitchoverReadReplicaMessageRequestTypeDef = TypedDict(
     "SwitchoverReadReplicaMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 
@@ -2399,22 +2338,20 @@
     "_OptionalCopyDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCopyDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCopyDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCopyDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBClusterSnapshotMessageRequestTypeDef",
     {
         "SourceDBClusterSnapshotIdentifier": str,
         "TargetDBClusterSnapshotIdentifier": str,
     },
 )
@@ -2426,22 +2363,20 @@
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class CopyDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCopyDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCopyDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCopyDBParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBParameterGroupMessageRequestTypeDef",
     {
         "SourceDBParameterGroupIdentifier": str,
         "TargetDBParameterGroupIdentifier": str,
         "TargetDBParameterGroupDescription": str,
     },
@@ -2450,22 +2385,20 @@
     "_OptionalCopyDBParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyDBParameterGroupMessageRequestTypeDef(
     _RequiredCopyDBParameterGroupMessageRequestTypeDef,
     _OptionalCopyDBParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCopyDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBSnapshotMessageRequestTypeDef",
     {
         "SourceDBSnapshotIdentifier": str,
         "TargetDBSnapshotIdentifier": str,
     },
 )
@@ -2480,21 +2413,19 @@
         "TargetCustomAvailabilityZone": str,
         "CopyOptionGroup": bool,
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class CopyDBSnapshotMessageRequestTypeDef(
     _RequiredCopyDBSnapshotMessageRequestTypeDef, _OptionalCopyDBSnapshotMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCopyOptionGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCopyOptionGroupMessageRequestTypeDef",
     {
         "SourceOptionGroupIdentifier": str,
         "TargetOptionGroupIdentifier": str,
         "TargetOptionGroupDescription": str,
     },
@@ -2503,21 +2434,19 @@
     "_OptionalCopyOptionGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyOptionGroupMessageRequestTypeDef(
     _RequiredCopyOptionGroupMessageRequestTypeDef, _OptionalCopyOptionGroupMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBlueGreenDeploymentRequestRequestTypeDef",
     {
         "BlueGreenDeploymentName": str,
         "Source": str,
     },
 )
@@ -2528,22 +2457,20 @@
         "TargetDBParameterGroupName": str,
         "TargetDBClusterParameterGroupName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredCreateBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalCreateBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
@@ -2557,22 +2484,20 @@
         "Description": str,
         "Manifest": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCustomDBEngineVersionMessageRequestTypeDef(
     _RequiredCreateCustomDBEngineVersionMessageRequestTypeDef,
     _OptionalCreateCustomDBEngineVersionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "EndpointType": str,
     },
@@ -2583,22 +2508,20 @@
         "StaticMembers": Sequence[str],
         "ExcludedMembers": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBClusterEndpointMessageRequestTypeDef(
     _RequiredCreateDBClusterEndpointMessageRequestTypeDef,
     _OptionalCreateDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
     },
@@ -2607,22 +2530,20 @@
     "_OptionalCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCreateDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterIdentifier": str,
     },
 )
@@ -2630,22 +2551,20 @@
     "_OptionalCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCreateDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCreateDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBParameterGroupMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
     },
@@ -2654,22 +2573,20 @@
     "_OptionalCreateDBParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBParameterGroupMessageRequestTypeDef(
     _RequiredCreateDBParameterGroupMessageRequestTypeDef,
     _OptionalCreateDBParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBProxyEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDBProxyEndpointRequestRequestTypeDef",
     {
         "DBProxyName": str,
         "DBProxyEndpointName": str,
         "VpcSubnetIds": Sequence[str],
     },
@@ -2680,22 +2597,20 @@
         "VpcSecurityGroupIds": Sequence[str],
         "TargetRole": DBProxyEndpointTargetRoleType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBProxyEndpointRequestRequestTypeDef(
     _RequiredCreateDBProxyEndpointRequestRequestTypeDef,
     _OptionalCreateDBProxyEndpointRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSecurityGroupMessageRequestTypeDef",
     {
         "DBSecurityGroupName": str,
         "DBSecurityGroupDescription": str,
     },
 )
@@ -2703,22 +2618,20 @@
     "_OptionalCreateDBSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBSecurityGroupMessageRequestTypeDef(
     _RequiredCreateDBSecurityGroupMessageRequestTypeDef,
     _OptionalCreateDBSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSnapshotMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "DBInstanceIdentifier": str,
     },
 )
@@ -2726,21 +2639,19 @@
     "_OptionalCreateDBSnapshotMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBSnapshotMessageRequestTypeDef(
     _RequiredCreateDBSnapshotMessageRequestTypeDef, _OptionalCreateDBSnapshotMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -2749,22 +2660,20 @@
     "_OptionalCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBSubnetGroupMessageRequestTypeDef(
     _RequiredCreateDBSubnetGroupMessageRequestTypeDef,
     _OptionalCreateDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "SnsTopicArn": str,
     },
 )
@@ -2776,22 +2685,20 @@
         "SourceIds": Sequence[str],
         "Enabled": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateOptionGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateOptionGroupMessageRequestTypeDef",
     {
         "OptionGroupName": str,
         "EngineName": str,
         "MajorEngineVersion": str,
         "OptionGroupDescription": str,
@@ -2801,21 +2708,19 @@
     "_OptionalCreateOptionGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateOptionGroupMessageRequestTypeDef(
     _RequiredCreateOptionGroupMessageRequestTypeDef, _OptionalCreateOptionGroupMessageRequestTypeDef
 ):
     pass
 
-
 DBClusterSnapshotTypeDef = TypedDict(
     "DBClusterSnapshotTypeDef",
     {
         "AvailabilityZones": List[str],
         "DBClusterSnapshotIdentifier": str,
         "DBClusterIdentifier": str,
         "SnapshotCreateTime": datetime,
@@ -2835,14 +2740,15 @@
         "KmsKeyId": str,
         "DBClusterSnapshotArn": str,
         "SourceDBClusterSnapshotArn": str,
         "IAMDatabaseAuthenticationEnabled": bool,
         "TagList": List[TagTypeDef],
         "DBSystemId": str,
         "StorageType": str,
+        "DbClusterResourceId": str,
     },
     total=False,
 )
 
 _RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef",
     {
@@ -2855,22 +2761,20 @@
         "ReservedDBInstanceId": str,
         "DBInstanceCount": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PurchaseReservedDBInstancesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedDBInstancesOfferingMessageRequestTypeDef,
 ):
     pass
 
-
 TagListMessageTypeDef = TypedDict(
     "TagListMessageTypeDef",
     {
         "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2929,22 +2833,20 @@
     {
         "Force": bool,
         "UseEarliestTimeOnPointInTimeUnavailable": bool,
     },
     total=False,
 )
 
-
 class BacktrackDBClusterMessageRequestTypeDef(
     _RequiredBacktrackDBClusterMessageRequestTypeDef,
     _OptionalBacktrackDBClusterMessageRequestTypeDef,
 ):
     pass
 
-
 BlueGreenDeploymentTypeDef = TypedDict(
     "BlueGreenDeploymentTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
         "BlueGreenDeploymentName": str,
         "Source": str,
         "Target": str,
@@ -3019,22 +2921,20 @@
     {
         "ConnectionPoolConfig": ConnectionPoolConfigurationTypeDef,
         "NewName": str,
     },
     total=False,
 )
 
-
 class ModifyDBProxyTargetGroupRequestRequestTypeDef(
     _RequiredModifyDBProxyTargetGroupRequestRequestTypeDef,
     _OptionalModifyDBProxyTargetGroupRequestRequestTypeDef,
 ):
     pass
 
-
 CopyDBClusterParameterGroupResultTypeDef = TypedDict(
     "CopyDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3134,26 +3034,25 @@
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
         "DBSystemId": str,
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
+        "EnableLocalWriteForwarding": bool,
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class CreateDBClusterMessageRequestTypeDef(
     _RequiredCreateDBClusterMessageRequestTypeDef, _OptionalCreateDBClusterMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalModifyDBClusterMessageRequestTypeDef = TypedDict(
@@ -3195,25 +3094,24 @@
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
         "ManageMasterUserPassword": bool,
         "RotateMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "EngineMode": str,
         "AllowEngineModeChange": bool,
+        "EnableLocalWriteForwarding": bool,
     },
     total=False,
 )
 
-
 class ModifyDBClusterMessageRequestTypeDef(
     _RequiredModifyDBClusterMessageRequestTypeDef, _OptionalModifyDBClusterMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredRestoreDBClusterFromS3MessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterFromS3MessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Engine": str,
         "MasterUsername": str,
         "SourceEngine": str,
@@ -3254,22 +3152,20 @@
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "StorageType": str,
     },
     total=False,
 )
 
-
 class RestoreDBClusterFromS3MessageRequestTypeDef(
     _RequiredRestoreDBClusterFromS3MessageRequestTypeDef,
     _OptionalRestoreDBClusterFromS3MessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "Engine": str,
     },
@@ -3302,33 +3198,31 @@
         "PubliclyAccessible": bool,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
     },
     total=False,
 )
 
-
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
-        "SourceDBClusterIdentifier": str,
     },
 )
 _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
     "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
         "RestoreType": str,
+        "SourceDBClusterIdentifier": str,
         "RestoreToTime": TimestampTypeDef,
         "UseLatestRestorableTime": bool,
         "Port": int,
         "DBSubnetGroupName": str,
         "OptionGroupName": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
@@ -3345,26 +3239,25 @@
         "EngineMode": str,
         "DBClusterInstanceClass": str,
         "StorageType": str,
         "PubliclyAccessible": bool,
         "Iops": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
+        "SourceDbClusterResourceId": str,
     },
     total=False,
 )
 
-
 class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
     _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
     _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "Engine": str,
     },
@@ -3398,14 +3291,18 @@
         "DBClusterIdentifier": str,
         "StorageType": str,
         "TdeCredentialArn": str,
         "TdeCredentialPassword": str,
         "StorageEncrypted": bool,
         "KmsKeyId": str,
         "Domain": str,
+        "DomainFqdn": str,
+        "DomainOu": str,
+        "DomainAuthSecretArn": str,
+        "DomainDnsIps": Sequence[str],
         "CopyTagsToSnapshot": bool,
         "MonitoringInterval": int,
         "MonitoringRoleArn": str,
         "DomainIAMRoleName": str,
         "PromotionTier": int,
         "Timezone": str,
         "EnableIAMDatabaseAuthentication": bool,
@@ -3420,25 +3317,24 @@
         "CustomIamInstanceProfile": str,
         "BackupTarget": str,
         "NetworkType": str,
         "StorageThroughput": int,
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "CACertificateIdentifier": str,
+        "DBSystemId": str,
     },
     total=False,
 )
 
-
 class CreateDBInstanceMessageRequestTypeDef(
     _RequiredCreateDBInstanceMessageRequestTypeDef, _OptionalCreateDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalCreateDBInstanceReadReplicaMessageRequestTypeDef = TypedDict(
@@ -3469,35 +3365,37 @@
         "PerformanceInsightsRetentionPeriod": int,
         "EnableCloudwatchLogsExports": Sequence[str],
         "ProcessorFeatures": Sequence[ProcessorFeatureTypeDef],
         "UseDefaultProcessorFeatures": bool,
         "DeletionProtection": bool,
         "Domain": str,
         "DomainIAMRoleName": str,
+        "DomainFqdn": str,
+        "DomainOu": str,
+        "DomainAuthSecretArn": str,
+        "DomainDnsIps": Sequence[str],
         "ReplicaMode": ReplicaModeType,
         "MaxAllocatedStorage": int,
         "CustomIamInstanceProfile": str,
         "NetworkType": str,
         "StorageThroughput": int,
         "EnableCustomerOwnedIp": bool,
         "AllocatedStorage": int,
         "SourceDBClusterIdentifier": str,
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class CreateDBInstanceReadReplicaMessageRequestTypeDef(
     _RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef,
     _OptionalCreateDBInstanceReadReplicaMessageRequestTypeDef,
 ):
     pass
 
-
 DBSnapshotTypeDef = TypedDict(
     "DBSnapshotTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "DBInstanceIdentifier": str,
         "SnapshotCreateTime": datetime,
         "Engine": str,
@@ -3526,14 +3424,15 @@
         "ProcessorFeatures": List[ProcessorFeatureTypeDef],
         "DbiResourceId": str,
         "TagList": List[TagTypeDef],
         "OriginalSnapshotCreateTime": datetime,
         "SnapshotDatabaseTime": datetime,
         "SnapshotTarget": str,
         "StorageThroughput": int,
+        "DBSystemId": str,
     },
     total=False,
 )
 
 _RequiredModifyDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBInstanceMessageRequestTypeDef",
     {
@@ -3563,20 +3462,25 @@
         "OptionGroupName": str,
         "NewDBInstanceIdentifier": str,
         "StorageType": str,
         "TdeCredentialArn": str,
         "TdeCredentialPassword": str,
         "CACertificateIdentifier": str,
         "Domain": str,
+        "DomainFqdn": str,
+        "DomainOu": str,
+        "DomainAuthSecretArn": str,
+        "DomainDnsIps": Sequence[str],
         "CopyTagsToSnapshot": bool,
         "MonitoringInterval": int,
         "DBPortNumber": int,
         "PubliclyAccessible": bool,
         "MonitoringRoleArn": str,
         "DomainIAMRoleName": str,
+        "DisableDomain": bool,
         "PromotionTier": int,
         "EnableIAMDatabaseAuthentication": bool,
         "EnablePerformanceInsights": bool,
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "CloudwatchLogsExportConfiguration": CloudwatchLogsExportConfigurationTypeDef,
         "ProcessorFeatures": Sequence[ProcessorFeatureTypeDef],
@@ -3595,21 +3499,19 @@
         "RotateMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "Engine": str,
     },
     total=False,
 )
 
-
 class ModifyDBInstanceMessageRequestTypeDef(
     _RequiredModifyDBInstanceMessageRequestTypeDef, _OptionalModifyDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 PendingModifiedValuesTypeDef = TypedDict(
     "PendingModifiedValuesTypeDef",
     {
         "DBInstanceClass": str,
         "AllocatedStorage": int,
         "MasterUserPassword": str,
         "Port": int,
@@ -3657,14 +3559,18 @@
         "OptionGroupName": str,
         "Tags": Sequence[TagTypeDef],
         "StorageType": str,
         "TdeCredentialArn": str,
         "TdeCredentialPassword": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Domain": str,
+        "DomainFqdn": str,
+        "DomainOu": str,
+        "DomainAuthSecretArn": str,
+        "DomainDnsIps": Sequence[str],
         "CopyTagsToSnapshot": bool,
         "DomainIAMRoleName": str,
         "EnableIAMDatabaseAuthentication": bool,
         "EnableCloudwatchLogsExports": Sequence[str],
         "ProcessorFeatures": Sequence[ProcessorFeatureTypeDef],
         "UseDefaultProcessorFeatures": bool,
         "DBParameterGroupName": str,
@@ -3676,22 +3582,20 @@
         "StorageThroughput": int,
         "DBClusterSnapshotIdentifier": str,
         "AllocatedStorage": int,
     },
     total=False,
 )
 
-
 class RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreDBInstanceFromS3MessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceFromS3MessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "Engine": str,
         "SourceEngine": str,
@@ -3744,22 +3648,20 @@
         "StorageThroughput": int,
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
     },
     total=False,
 )
 
-
 class RestoreDBInstanceFromS3MessageRequestTypeDef(
     _RequiredRestoreDBInstanceFromS3MessageRequestTypeDef,
     _OptionalRestoreDBInstanceFromS3MessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     {
         "TargetDBInstanceIdentifier": str,
     },
 )
 _OptionalRestoreDBInstanceToPointInTimeMessageRequestTypeDef = TypedDict(
@@ -3784,14 +3686,18 @@
         "Tags": Sequence[TagTypeDef],
         "StorageType": str,
         "TdeCredentialArn": str,
         "TdeCredentialPassword": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Domain": str,
         "DomainIAMRoleName": str,
+        "DomainFqdn": str,
+        "DomainOu": str,
+        "DomainAuthSecretArn": str,
+        "DomainDnsIps": Sequence[str],
         "EnableIAMDatabaseAuthentication": bool,
         "EnableCloudwatchLogsExports": Sequence[str],
         "ProcessorFeatures": Sequence[ProcessorFeatureTypeDef],
         "UseDefaultProcessorFeatures": bool,
         "DBParameterGroupName": str,
         "DeletionProtection": bool,
         "SourceDbiResourceId": str,
@@ -3803,22 +3709,20 @@
         "NetworkType": str,
         "StorageThroughput": int,
         "AllocatedStorage": int,
     },
     total=False,
 )
 
-
 class RestoreDBInstanceToPointInTimeMessageRequestTypeDef(
     _RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef,
     _OptionalRestoreDBInstanceToPointInTimeMessageRequestTypeDef,
 ):
     pass
 
-
 CreateDBProxyEndpointResponseTypeDef = TypedDict(
     "CreateDBProxyEndpointResponseTypeDef",
     {
         "DBProxyEndpoint": DBProxyEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3866,21 +3770,19 @@
         "IdleClientTimeout": int,
         "DebugLogging": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBProxyRequestRequestTypeDef(
     _RequiredCreateDBProxyRequestRequestTypeDef, _OptionalCreateDBProxyRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyDBProxyRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDBProxyRequestRequestTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalModifyDBProxyRequestRequestTypeDef = TypedDict(
@@ -3893,20 +3795,48 @@
         "DebugLogging": bool,
         "RoleArn": str,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyDBProxyRequestRequestTypeDef(
     _RequiredModifyDBProxyRequestRequestTypeDef, _OptionalModifyDBProxyRequestRequestTypeDef
 ):
     pass
 
+DBClusterAutomatedBackupTypeDef = TypedDict(
+    "DBClusterAutomatedBackupTypeDef",
+    {
+        "Engine": str,
+        "VpcId": str,
+        "DBClusterAutomatedBackupsArn": str,
+        "DBClusterIdentifier": str,
+        "RestoreWindow": RestoreWindowTypeDef,
+        "MasterUsername": str,
+        "DbClusterResourceId": str,
+        "Region": str,
+        "LicenseModel": str,
+        "Status": str,
+        "IAMDatabaseAuthenticationEnabled": bool,
+        "ClusterCreateTime": datetime,
+        "StorageEncrypted": bool,
+        "AllocatedStorage": int,
+        "EngineVersion": str,
+        "DBClusterArn": str,
+        "BackupRetentionPeriod": int,
+        "EngineMode": str,
+        "AvailabilityZones": List[str],
+        "Port": int,
+        "KmsKeyId": str,
+        "StorageType": str,
+        "Iops": int,
+    },
+    total=False,
+)
 
 DBClusterBacktrackMessageTypeDef = TypedDict(
     "DBClusterBacktrackMessageTypeDef",
     {
         "Marker": str,
         "DBClusterBacktracks": List[DBClusterBacktrackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3921,39 +3851,97 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBParameterGroupDetailsTypeDef = TypedDict(
     "DBParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
+    },
+    total=False,
+)
+
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
     },
     total=False,
 )
 
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+    },
+)
+_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+class ResetDBParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBParameterGroupMessageRequestTypeDef,
+):
+    pass
+
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
     total=False,
@@ -3989,14 +3977,15 @@
         "KMSKeyId": str,
         "CreateTime": datetime,
         "TagList": List[TagTypeDef],
         "SupportsBabelfish": bool,
         "CustomDBEngineVersionManifest": str,
         "SupportsCertificateRotationWithoutRestart": bool,
         "SupportedCACertificateIdentifiers": List[str],
+        "SupportsLocalWriteForwarding": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBEngineVersionTypeDef = TypedDict(
     "DBEngineVersionTypeDef",
     {
@@ -4027,14 +4016,15 @@
         "KMSKeyId": str,
         "CreateTime": datetime,
         "TagList": List[TagTypeDef],
         "SupportsBabelfish": bool,
         "CustomDBEngineVersionManifest": str,
         "SupportsCertificateRotationWithoutRestart": bool,
         "SupportedCACertificateIdentifiers": List[str],
+        "SupportsLocalWriteForwarding": bool,
     },
     total=False,
 )
 
 DBInstanceAutomatedBackupTypeDef = TypedDict(
     "DBInstanceAutomatedBackupTypeDef",
     {
@@ -4150,14 +4140,26 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeDBClusterAutomatedBackupsMessageRequestTypeDef = TypedDict(
+    "DescribeDBClusterAutomatedBackupsMessageRequestTypeDef",
+    {
+        "DbClusterResourceId": str,
+        "DBClusterIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
 _RequiredDescribeDBClusterBacktracksMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBClusterBacktracksMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalDescribeDBClusterBacktracksMessageRequestTypeDef = TypedDict(
@@ -4167,22 +4169,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeDBClusterBacktracksMessageRequestTypeDef(
     _RequiredDescribeDBClusterBacktracksMessageRequestTypeDef,
     _OptionalDescribeDBClusterBacktracksMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeDBClusterEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
@@ -4215,33 +4215,32 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeDBClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDBClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDBClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeDBClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
+        "DbClusterResourceId": str,
     },
     total=False,
 )
 
 DescribeDBClustersMessageRequestTypeDef = TypedDict(
     "DescribeDBClustersMessageRequestTypeDef",
     {
@@ -4310,22 +4309,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeDBLogFilesMessageRequestTypeDef(
     _RequiredDescribeDBLogFilesMessageRequestTypeDef,
     _OptionalDescribeDBLogFilesMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeDBParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBParameterGroupsMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -4346,22 +4343,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeDBParametersMessageRequestTypeDef(
     _RequiredDescribeDBParametersMessageRequestTypeDef,
     _OptionalDescribeDBParametersMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeDBProxiesRequestRequestTypeDef = TypedDict(
     "DescribeDBProxiesRequestRequestTypeDef",
     {
         "DBProxyName": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4394,22 +4389,20 @@
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-
 class DescribeDBProxyTargetGroupsRequestRequestTypeDef(
     _RequiredDescribeDBProxyTargetGroupsRequestRequestTypeDef,
     _OptionalDescribeDBProxyTargetGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeDBProxyTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDBProxyTargetsRequestRequestTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalDescribeDBProxyTargetsRequestRequestTypeDef = TypedDict(
@@ -4419,22 +4412,20 @@
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-
 class DescribeDBProxyTargetsRequestRequestTypeDef(
     _RequiredDescribeDBProxyTargetsRequestRequestTypeDef,
     _OptionalDescribeDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeDBSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBSecurityGroupsMessageRequestTypeDef",
     {
         "DBSecurityGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -4481,22 +4472,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
         "DBParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -4505,22 +4494,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeEventCategoriesMessageRequestTypeDef = TypedDict(
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
@@ -4590,22 +4577,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeOptionGroupOptionsMessageRequestTypeDef(
     _RequiredDescribeOptionGroupOptionsMessageRequestTypeDef,
     _OptionalDescribeOptionGroupOptionsMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeOptionGroupsMessageRequestTypeDef = TypedDict(
     "DescribeOptionGroupsMessageRequestTypeDef",
     {
         "OptionGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4632,22 +4617,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
 ):
     pass
 
-
 DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4710,22 +4693,20 @@
     "_OptionalListTagsForResourceMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
 class ListTagsForResourceMessageRequestTypeDef(
     _RequiredListTagsForResourceMessageRequestTypeDef,
     _OptionalListTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeBlueGreenDeploymentsRequestDescribeBlueGreenDeploymentsPaginateTypeDef = TypedDict(
     "DescribeBlueGreenDeploymentsRequestDescribeBlueGreenDeploymentsPaginateTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4754,22 +4735,20 @@
         "BacktrackIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef(
     _RequiredDescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef,
     _OptionalDescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -4799,31 +4778,30 @@
         "Source": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
     _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "IncludeShared": bool,
         "IncludePublic": bool,
+        "DbClusterResourceId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
     "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
@@ -4888,22 +4866,20 @@
         "FileSize": int,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef(
     _RequiredDescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef,
     _OptionalDescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
     "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     {
         "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4922,22 +4898,20 @@
         "Source": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
     _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBProxiesRequestDescribeDBProxiesPaginateTypeDef = TypedDict(
     "DescribeDBProxiesRequestDescribeDBProxiesPaginateTypeDef",
     {
         "DBProxyName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4967,22 +4941,20 @@
         "TargetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef(
     _RequiredDescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef,
     _OptionalDescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef = TypedDict(
@@ -4991,22 +4963,20 @@
         "TargetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef(
     _RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef,
     _OptionalDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBSecurityGroupsMessageDescribeDBSecurityGroupsPaginateTypeDef = TypedDict(
     "DescribeDBSecurityGroupsMessageDescribeDBSecurityGroupsPaginateTypeDef",
     {
         "DBSecurityGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -5049,22 +5019,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     {
         "DBParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
@@ -5072,22 +5040,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
 ):
     pass
 
-
 DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -5143,22 +5109,20 @@
         "MajorEngineVersion": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef(
     _RequiredDescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef,
     _OptionalDescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef,
 ):
     pass
 
-
 DescribeOptionGroupsMessageDescribeOptionGroupsPaginateTypeDef = TypedDict(
     "DescribeOptionGroupsMessageDescribeOptionGroupsPaginateTypeDef",
     {
         "OptionGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "EngineName": str,
         "MajorEngineVersion": str,
@@ -5183,22 +5147,20 @@
         "Vpc": bool,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
 ):
     pass
 
-
 DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
     TypedDict(
         "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
         {
             "ResourceIdentifier": str,
             "Filters": Sequence[FilterTypeDef],
             "PaginationConfig": PaginatorConfigTypeDef,
@@ -5260,33 +5222,32 @@
     "_OptionalDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef(
     _RequiredDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef,
     _OptionalDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef,
 ):
     pass
 
-
 DescribeDBClusterSnapshotsMessageDBClusterSnapshotAvailableWaitTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDBClusterSnapshotAvailableWaitTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
+        "DbClusterResourceId": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClusterSnapshotsMessageDBClusterSnapshotDeletedWaitTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDBClusterSnapshotDeletedWaitTypeDef",
@@ -5295,14 +5256,15 @@
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
+        "DbClusterResourceId": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClustersMessageDBClusterAvailableWaitTypeDef = TypedDict(
     "DescribeDBClustersMessageDBClusterAvailableWaitTypeDef",
@@ -5487,21 +5449,19 @@
         "DBSecurityGroupMemberships": Sequence[str],
         "VpcSecurityGroupMemberships": Sequence[str],
         "OptionSettings": Sequence[OptionSettingTypeDef],
     },
     total=False,
 )
 
-
 class OptionConfigurationTypeDef(
     _RequiredOptionConfigurationTypeDef, _OptionalOptionConfigurationTypeDef
 ):
     pass
 
-
 OptionTypeDef = TypedDict(
     "OptionTypeDef",
     {
         "OptionName": str,
         "OptionDescription": str,
         "Persistent": bool,
         "Permanent": bool,
@@ -5521,15 +5481,14 @@
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetOutpost": OutpostTypeDef,
         "SubnetStatus": str,
     },
     total=False,
 )
 
-ParameterUnionTypeDef = Union[ParameterTypeDef, ParameterOutputTypeDef]
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -5744,14 +5703,15 @@
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationInfoTypeDef,
         "NetworkType": str,
         "DBSystemId": str,
         "MasterUserSecret": MasterUserSecretTypeDef,
         "IOOptimizedNextAllowedModificationTime": datetime,
+        "LocalWriteForwardingStatus": LocalWriteForwardingStatusType,
     },
     total=False,
 )
 
 DescribeDBProxyTargetGroupsResponseTypeDef = TypedDict(
     "DescribeDBProxyTargetGroupsResponseTypeDef",
     {
@@ -5806,14 +5766,31 @@
     "ModifyDBSnapshotResultTypeDef",
     {
         "DBSnapshot": DBSnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DBClusterAutomatedBackupMessageTypeDef = TypedDict(
+    "DBClusterAutomatedBackupMessageTypeDef",
+    {
+        "Marker": str,
+        "DBClusterAutomatedBackups": List[DBClusterAutomatedBackupTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDBClusterAutomatedBackupResultTypeDef = TypedDict(
+    "DeleteDBClusterAutomatedBackupResultTypeDef",
+    {
+        "DBClusterAutomatedBackup": DBClusterAutomatedBackupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6068,21 +6045,19 @@
         "OptionsToInclude": Sequence[OptionConfigurationTypeDef],
         "OptionsToRemove": Sequence[str],
         "ApplyImmediately": bool,
     },
     total=False,
 )
 
-
 class ModifyOptionGroupMessageRequestTypeDef(
     _RequiredModifyOptionGroupMessageRequestTypeDef, _OptionalModifyOptionGroupMessageRequestTypeDef
 ):
     pass
 
-
 OptionGroupTypeDef = TypedDict(
     "OptionGroupTypeDef",
     {
         "OptionGroupName": str,
         "OptionGroupDescription": str,
         "EngineName": str,
         "MajorEngineVersion": str,
@@ -6107,76 +6082,14 @@
         "Subnets": List[SubnetTypeDef],
         "DBSubnetGroupArn": str,
         "SupportedNetworkTypes": List[str],
     },
     total=False,
 )
 
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-)
-
-ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-)
-
-_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class ResetDBClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
-
-
-_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-    },
-)
-_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class ResetDBParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBParameterGroupMessageRequestTypeDef,
-):
-    pass
-
-
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6454,14 +6367,15 @@
         "NetworkType": str,
         "ActivityStreamPolicyStatus": ActivityStreamPolicyStatusType,
         "StorageThroughput": int,
         "DBSystemId": str,
         "MasterUserSecret": MasterUserSecretTypeDef,
         "CertificateDetails": CertificateDetailsTypeDef,
         "ReadReplicaSourceDBClusterIdentifier": str,
+        "PercentProgress": str,
     },
     total=False,
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
```

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/type_defs.pyi` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     DBProxyEndpointStatusType,
     DBProxyEndpointTargetRoleType,
     DBProxyStatusType,
     EngineFamilyType,
     ExportSourceTypeType,
     FailoverStatusType,
     IAMAuthModeType,
+    LocalWriteForwardingStatusType,
     ReplicaModeType,
     SourceTypeType,
     TargetHealthReasonType,
     TargetRoleType,
     TargetStateType,
     TargetTypeType,
     WriteForwardingStatusType,
@@ -45,14 +46,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountQuotaTypeDef",
     "ResponseMetadataTypeDef",
     "AddRoleToDBClusterMessageRequestTypeDef",
     "AddRoleToDBInstanceMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
@@ -78,43 +80,44 @@
     "ScalingConfigurationTypeDef",
     "ServerlessV2ScalingConfigurationTypeDef",
     "ProcessorFeatureTypeDef",
     "DBProxyEndpointTypeDef",
     "UserAuthConfigTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "CustomDBEngineVersionAMITypeDef",
+    "RestoreWindowTypeDef",
     "DBClusterBacktrackTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
-    "ParameterOutputTypeDef",
+    "ParameterTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "DomainMembershipTypeDef",
     "MasterUserSecretTypeDef",
     "ScalingConfigurationInfoTypeDef",
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "TimezoneTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceAutomatedBackupsReplicationTypeDef",
-    "RestoreWindowTypeDef",
     "DBInstanceRoleTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "DBParameterGroupStatusTypeDef",
     "DBSecurityGroupMembershipTypeDef",
     "EndpointTypeDef",
     "OptionGroupMembershipTypeDef",
     "TargetHealthTypeDef",
     "UserAuthConfigInfoTypeDef",
     "EC2SecurityGroupTypeDef",
     "IPRangeTypeDef",
     "DBSnapshotAttributeTypeDef",
     "DeleteBlueGreenDeploymentRequestRequestTypeDef",
     "DeleteCustomDBEngineVersionMessageRequestTypeDef",
+    "DeleteDBClusterAutomatedBackupMessageRequestTypeDef",
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceAutomatedBackupMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBParameterGroupMessageRequestTypeDef",
@@ -155,15 +158,14 @@
     "ModifyDBSnapshotMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "OptionSettingTypeDef",
     "OptionVersionTypeDef",
     "OutpostTypeDef",
-    "ParameterTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "PromoteReadReplicaMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBClusterMessageRequestTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RecurringChargeTypeDef",
@@ -254,29 +256,35 @@
     "RestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     "CreateDBProxyEndpointResponseTypeDef",
     "DeleteDBProxyEndpointResponseTypeDef",
     "DescribeDBProxyEndpointsResponseTypeDef",
     "ModifyDBProxyEndpointResponseTypeDef",
     "CreateDBProxyRequestRequestTypeDef",
     "ModifyDBProxyRequestRequestTypeDef",
+    "DBClusterAutomatedBackupTypeDef",
     "DBClusterBacktrackMessageTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionResponseTypeDef",
     "DBEngineVersionTypeDef",
     "DBInstanceAutomatedBackupTypeDef",
     "DBProxyTargetTypeDef",
     "DBProxyTypeDef",
     "DBSecurityGroupTypeDef",
     "DBSnapshotAttributesResultTypeDef",
     "DescribeBlueGreenDeploymentsRequestRequestTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
+    "DescribeDBClusterAutomatedBackupsMessageRequestTypeDef",
     "DescribeDBClusterBacktracksMessageRequestTypeDef",
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
@@ -356,15 +364,14 @@
     "EventsMessageTypeDef",
     "ExportTasksMessageTypeDef",
     "GlobalClusterTypeDef",
     "OptionGroupOptionSettingTypeDef",
     "OptionConfigurationTypeDef",
     "OptionTypeDef",
     "SubnetTypeDef",
-    "ParameterUnionTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
     "ReservedDBInstanceTypeDef",
     "ReservedDBInstancesOfferingTypeDef",
     "SourceRegionMessageTypeDef",
     "CopyDBClusterSnapshotResultTypeDef",
     "CreateDBClusterSnapshotResultTypeDef",
@@ -379,14 +386,16 @@
     "DescribeDBProxyTargetGroupsResponseTypeDef",
     "ModifyDBProxyTargetGroupResponseTypeDef",
     "CopyDBSnapshotResultTypeDef",
     "CreateDBSnapshotResultTypeDef",
     "DBSnapshotMessageTypeDef",
     "DeleteDBSnapshotResultTypeDef",
     "ModifyDBSnapshotResultTypeDef",
+    "DBClusterAutomatedBackupMessageTypeDef",
+    "DeleteDBClusterAutomatedBackupResultTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     "DBEngineVersionMessageTypeDef",
     "DBInstanceAutomatedBackupMessageTypeDef",
     "DeleteDBInstanceAutomatedBackupResultTypeDef",
@@ -410,18 +419,14 @@
     "GlobalClustersMessageTypeDef",
     "ModifyGlobalClusterResultTypeDef",
     "RemoveFromGlobalClusterResultTypeDef",
     "OptionGroupOptionTypeDef",
     "ModifyOptionGroupMessageRequestTypeDef",
     "OptionGroupTypeDef",
     "DBSubnetGroupTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBParameterGroupMessageRequestTypeDef",
     "ApplyPendingMaintenanceActionResultTypeDef",
     "PendingMaintenanceActionsMessageTypeDef",
     "ValidDBInstanceModificationsMessageTypeDef",
     "PurchaseReservedDBInstancesOfferingResultTypeDef",
     "ReservedDBInstanceMessageTypeDef",
     "ReservedDBInstancesOfferingMessageTypeDef",
     "CreateDBClusterResultTypeDef",
@@ -493,20 +498,22 @@
     "_OptionalAddRoleToDBClusterMessageRequestTypeDef",
     {
         "FeatureName": str,
     },
     total=False,
 )
 
+
 class AddRoleToDBClusterMessageRequestTypeDef(
     _RequiredAddRoleToDBClusterMessageRequestTypeDef,
     _OptionalAddRoleToDBClusterMessageRequestTypeDef,
 ):
     pass
 
+
 AddRoleToDBInstanceMessageRequestTypeDef = TypedDict(
     "AddRoleToDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "RoleArn": str,
         "FeatureName": str,
     },
@@ -568,20 +575,22 @@
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupId": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+
 class AuthorizeDBSecurityGroupIngressMessageRequestTypeDef(
     _RequiredAuthorizeDBSecurityGroupIngressMessageRequestTypeDef,
     _OptionalAuthorizeDBSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
+
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -668,20 +677,22 @@
     "_OptionalClientGenerateDbAuthTokenRequestTypeDef",
     {
         "Region": Optional[str],
     },
     total=False,
 )
 
+
 class ClientGenerateDbAuthTokenRequestTypeDef(
     _RequiredClientGenerateDbAuthTokenRequestTypeDef,
     _OptionalClientGenerateDbAuthTokenRequestTypeDef,
 ):
     pass
 
+
 CloudwatchLogsExportConfigurationTypeDef = TypedDict(
     "CloudwatchLogsExportConfigurationTypeDef",
     {
         "EnableLogTypes": Sequence[str],
         "DisableLogTypes": Sequence[str],
     },
     total=False,
@@ -823,14 +834,23 @@
     {
         "ImageId": str,
         "Status": str,
     },
     total=False,
 )
 
+RestoreWindowTypeDef = TypedDict(
+    "RestoreWindowTypeDef",
+    {
+        "EarliestTime": datetime,
+        "LatestTime": datetime,
+    },
+    total=False,
+)
+
 DBClusterBacktrackTypeDef = TypedDict(
     "DBClusterBacktrackTypeDef",
     {
         "DBClusterIdentifier": str,
         "BacktrackIdentifier": str,
         "BacktrackTo": datetime,
         "BacktrackedFrom": datetime,
@@ -873,16 +893,16 @@
     {
         "DBClusterOptionGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "ApplyType": str,
         "DataType": str,
@@ -917,14 +937,17 @@
 DomainMembershipTypeDef = TypedDict(
     "DomainMembershipTypeDef",
     {
         "Domain": str,
         "Status": str,
         "FQDN": str,
         "IAMRoleName": str,
+        "OU": str,
+        "AuthSecretArn": str,
+        "DnsIps": List[str],
     },
     total=False,
 )
 
 MasterUserSecretTypeDef = TypedDict(
     "MasterUserSecretTypeDef",
     {
@@ -982,35 +1005,27 @@
         "Description": str,
         "AutoUpgrade": bool,
         "IsMajorVersionUpgrade": bool,
         "SupportedEngineModes": List[str],
         "SupportsParallelQuery": bool,
         "SupportsGlobalDatabases": bool,
         "SupportsBabelfish": bool,
+        "SupportsLocalWriteForwarding": bool,
     },
     total=False,
 )
 
 DBInstanceAutomatedBackupsReplicationTypeDef = TypedDict(
     "DBInstanceAutomatedBackupsReplicationTypeDef",
     {
         "DBInstanceAutomatedBackupsArn": str,
     },
     total=False,
 )
 
-RestoreWindowTypeDef = TypedDict(
-    "RestoreWindowTypeDef",
-    {
-        "EarliestTime": datetime,
-        "LatestTime": datetime,
-    },
-    total=False,
-)
-
 DBInstanceRoleTypeDef = TypedDict(
     "DBInstanceRoleTypeDef",
     {
         "RoleArn": str,
         "FeatureName": str,
         "Status": str,
     },
@@ -1127,28 +1142,37 @@
     "_OptionalDeleteBlueGreenDeploymentRequestRequestTypeDef",
     {
         "DeleteTarget": bool,
     },
     total=False,
 )
 
+
 class DeleteBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredDeleteBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalDeleteBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "DeleteCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
 
+DeleteDBClusterAutomatedBackupMessageRequestTypeDef = TypedDict(
+    "DeleteDBClusterAutomatedBackupMessageRequestTypeDef",
+    {
+        "DbClusterResourceId": str,
+    },
+)
+
 DeleteDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 
@@ -1159,23 +1183,26 @@
     },
 )
 _OptionalDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_OptionalDeleteDBClusterMessageRequestTypeDef",
     {
         "SkipFinalSnapshot": bool,
         "FinalDBSnapshotIdentifier": str,
+        "DeleteAutomatedBackups": bool,
     },
     total=False,
 )
 
+
 class DeleteDBClusterMessageRequestTypeDef(
     _RequiredDeleteDBClusterMessageRequestTypeDef, _OptionalDeleteDBClusterMessageRequestTypeDef
 ):
     pass
 
+
 DeleteDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 
@@ -1207,19 +1234,21 @@
         "SkipFinalSnapshot": bool,
         "FinalDBSnapshotIdentifier": str,
         "DeleteAutomatedBackups": bool,
     },
     total=False,
 )
 
+
 class DeleteDBInstanceMessageRequestTypeDef(
     _RequiredDeleteDBInstanceMessageRequestTypeDef, _OptionalDeleteDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 DeleteDBParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteDBParameterGroupMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
     },
 )
 
@@ -1291,20 +1320,22 @@
         "TargetGroupName": str,
         "DBInstanceIdentifiers": Sequence[str],
         "DBClusterIdentifiers": Sequence[str],
     },
     total=False,
 )
 
+
 class DeregisterDBProxyTargetsRequestRequestTypeDef(
     _RequiredDeregisterDBProxyTargetsRequestRequestTypeDef,
     _OptionalDeregisterDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
@@ -1380,20 +1411,22 @@
     {
         "Marker": str,
         "NumberOfLines": int,
     },
     total=False,
 )
 
+
 class DownloadDBLogFilePortionMessageRequestTypeDef(
     _RequiredDownloadDBLogFilePortionMessageRequestTypeDef,
     _OptionalDownloadDBLogFilePortionMessageRequestTypeDef,
 ):
     pass
 
+
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
     total=False,
@@ -1445,19 +1478,21 @@
     "_OptionalFailoverDBClusterMessageRequestTypeDef",
     {
         "TargetDBInstanceIdentifier": str,
     },
     total=False,
 )
 
+
 class FailoverDBClusterMessageRequestTypeDef(
     _RequiredFailoverDBClusterMessageRequestTypeDef, _OptionalFailoverDBClusterMessageRequestTypeDef
 ):
     pass
 
+
 FailoverGlobalClusterMessageRequestTypeDef = TypedDict(
     "FailoverGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "TargetDbClusterIdentifier": str,
     },
 )
@@ -1522,20 +1557,22 @@
         "Capacity": int,
         "SecondsBeforeTimeout": int,
         "TimeoutAction": str,
     },
     total=False,
 )
 
+
 class ModifyCurrentDBClusterCapacityMessageRequestTypeDef(
     _RequiredModifyCurrentDBClusterCapacityMessageRequestTypeDef,
     _OptionalModifyCurrentDBClusterCapacityMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
@@ -1544,20 +1581,22 @@
     {
         "Description": str,
         "Status": CustomEngineVersionStatusType,
     },
     total=False,
 )
 
+
 class ModifyCustomDBEngineVersionMessageRequestTypeDef(
     _RequiredModifyCustomDBEngineVersionMessageRequestTypeDef,
     _OptionalModifyCustomDBEngineVersionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 _OptionalModifyDBClusterEndpointMessageRequestTypeDef = TypedDict(
@@ -1566,20 +1605,22 @@
         "EndpointType": str,
         "StaticMembers": Sequence[str],
         "ExcludedMembers": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyDBClusterEndpointMessageRequestTypeDef(
     _RequiredModifyDBClusterEndpointMessageRequestTypeDef,
     _OptionalModifyDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -1588,20 +1629,22 @@
     {
         "ValuesToAdd": Sequence[str],
         "ValuesToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyDBClusterSnapshotAttributeMessageRequestTypeDef(
     _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     _OptionalModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyDBProxyEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDBProxyEndpointRequestRequestTypeDef",
     {
         "DBProxyEndpointName": str,
     },
 )
 _OptionalModifyDBProxyEndpointRequestRequestTypeDef = TypedDict(
@@ -1609,20 +1652,22 @@
     {
         "NewDBProxyEndpointName": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyDBProxyEndpointRequestRequestTypeDef(
     _RequiredModifyDBProxyEndpointRequestRequestTypeDef,
     _OptionalModifyDBProxyEndpointRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyDBSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSnapshotAttributeMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -1631,20 +1676,22 @@
     {
         "ValuesToAdd": Sequence[str],
         "ValuesToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyDBSnapshotAttributeMessageRequestTypeDef(
     _RequiredModifyDBSnapshotAttributeMessageRequestTypeDef,
     _OptionalModifyDBSnapshotAttributeMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSnapshotMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
     },
 )
 _OptionalModifyDBSnapshotMessageRequestTypeDef = TypedDict(
@@ -1652,19 +1699,21 @@
     {
         "EngineVersion": str,
         "OptionGroupName": str,
     },
     total=False,
 )
 
+
 class ModifyDBSnapshotMessageRequestTypeDef(
     _RequiredModifyDBSnapshotMessageRequestTypeDef, _OptionalModifyDBSnapshotMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -1672,20 +1721,22 @@
     "_OptionalModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupDescription": str,
     },
     total=False,
 )
 
+
 class ModifyDBSubnetGroupMessageRequestTypeDef(
     _RequiredModifyDBSubnetGroupMessageRequestTypeDef,
     _OptionalModifyDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
     },
 )
 _OptionalModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
@@ -1695,20 +1746,22 @@
         "SourceType": str,
         "EventCategories": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class ModifyEventSubscriptionMessageRequestTypeDef(
     _RequiredModifyEventSubscriptionMessageRequestTypeDef,
     _OptionalModifyEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
+
 ModifyGlobalClusterMessageRequestTypeDef = TypedDict(
     "ModifyGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "NewGlobalClusterIdentifier": str,
         "DeletionProtection": bool,
         "EngineVersion": str,
@@ -1746,32 +1799,14 @@
     "OutpostTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterValue": str,
-        "Description": str,
-        "Source": str,
-        "ApplyType": str,
-        "DataType": str,
-        "AllowedValues": str,
-        "IsModifiable": bool,
-        "MinimumEngineVersion": str,
-        "ApplyMethod": ApplyMethodType,
-        "SupportedEngineModes": Sequence[str],
-    },
-    total=False,
-)
-
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
@@ -1799,20 +1834,22 @@
     {
         "BackupRetentionPeriod": int,
         "PreferredBackupWindow": str,
     },
     total=False,
 )
 
+
 class PromoteReadReplicaMessageRequestTypeDef(
     _RequiredPromoteReadReplicaMessageRequestTypeDef,
     _OptionalPromoteReadReplicaMessageRequestTypeDef,
 ):
     pass
 
+
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "From": int,
         "To": int,
         "Step": int,
     },
@@ -1836,19 +1873,21 @@
     "_OptionalRebootDBInstanceMessageRequestTypeDef",
     {
         "ForceFailover": bool,
     },
     total=False,
 )
 
+
 class RebootDBInstanceMessageRequestTypeDef(
     _RequiredRebootDBInstanceMessageRequestTypeDef, _OptionalRebootDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
     total=False,
@@ -1866,20 +1905,22 @@
         "TargetGroupName": str,
         "DBInstanceIdentifiers": Sequence[str],
         "DBClusterIdentifiers": Sequence[str],
     },
     total=False,
 )
 
+
 class RegisterDBProxyTargetsRequestRequestTypeDef(
     _RequiredRegisterDBProxyTargetsRequestRequestTypeDef,
     _OptionalRegisterDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 RemoveFromGlobalClusterMessageRequestTypeDef = TypedDict(
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "DbClusterIdentifier": str,
     },
     total=False,
@@ -1896,20 +1937,22 @@
     "_OptionalRemoveRoleFromDBClusterMessageRequestTypeDef",
     {
         "FeatureName": str,
     },
     total=False,
 )
 
+
 class RemoveRoleFromDBClusterMessageRequestTypeDef(
     _RequiredRemoveRoleFromDBClusterMessageRequestTypeDef,
     _OptionalRemoveRoleFromDBClusterMessageRequestTypeDef,
 ):
     pass
 
+
 RemoveRoleFromDBInstanceMessageRequestTypeDef = TypedDict(
     "RemoveRoleFromDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "RoleArn": str,
         "FeatureName": str,
     },
@@ -1944,20 +1987,22 @@
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupId": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+
 class RevokeDBSecurityGroupIngressMessageRequestTypeDef(
     _RequiredRevokeDBSecurityGroupIngressMessageRequestTypeDef,
     _OptionalRevokeDBSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
+
 SourceRegionTypeDef = TypedDict(
     "SourceRegionTypeDef",
     {
         "RegionName": str,
         "Endpoint": str,
         "Status": str,
         "SupportsDBInstanceAutomatedBackupsReplication": bool,
@@ -1978,20 +2023,22 @@
     {
         "ApplyImmediately": bool,
         "EngineNativeAuditFieldsIncluded": bool,
     },
     total=False,
 )
 
+
 class StartActivityStreamRequestRequestTypeDef(
     _RequiredStartActivityStreamRequestRequestTypeDef,
     _OptionalStartActivityStreamRequestRequestTypeDef,
 ):
     pass
 
+
 StartDBClusterMessageRequestTypeDef = TypedDict(
     "StartDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -2008,20 +2055,22 @@
         "KmsKeyId": str,
         "PreSignedUrl": str,
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class StartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef(
     _RequiredStartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef,
     _OptionalStartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef,
 ):
     pass
 
+
 StartDBInstanceMessageRequestTypeDef = TypedDict(
     "StartDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 
@@ -2040,39 +2089,43 @@
     {
         "S3Prefix": str,
         "ExportOnly": Sequence[str],
     },
     total=False,
 )
 
+
 class StartExportTaskMessageRequestTypeDef(
     _RequiredStartExportTaskMessageRequestTypeDef, _OptionalStartExportTaskMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredStopActivityStreamRequestRequestTypeDef = TypedDict(
     "_RequiredStopActivityStreamRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalStopActivityStreamRequestRequestTypeDef = TypedDict(
     "_OptionalStopActivityStreamRequestRequestTypeDef",
     {
         "ApplyImmediately": bool,
     },
     total=False,
 )
 
+
 class StopActivityStreamRequestRequestTypeDef(
     _RequiredStopActivityStreamRequestRequestTypeDef,
     _OptionalStopActivityStreamRequestRequestTypeDef,
 ):
     pass
 
+
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -2093,39 +2146,43 @@
     "_OptionalStopDBInstanceMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
     },
     total=False,
 )
 
+
 class StopDBInstanceMessageRequestTypeDef(
     _RequiredStopDBInstanceMessageRequestTypeDef, _OptionalStopDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
     },
 )
 _OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef",
     {
         "SwitchoverTimeout": int,
     },
     total=False,
 )
 
+
 class SwitchoverBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredSwitchoverBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalSwitchoverBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 SwitchoverReadReplicaMessageRequestTypeDef = TypedDict(
     "SwitchoverReadReplicaMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 
@@ -2340,20 +2397,22 @@
     "_OptionalCopyDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCopyDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCopyDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCopyDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBClusterSnapshotMessageRequestTypeDef",
     {
         "SourceDBClusterSnapshotIdentifier": str,
         "TargetDBClusterSnapshotIdentifier": str,
     },
 )
@@ -2365,20 +2424,22 @@
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class CopyDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCopyDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCopyDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCopyDBParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBParameterGroupMessageRequestTypeDef",
     {
         "SourceDBParameterGroupIdentifier": str,
         "TargetDBParameterGroupIdentifier": str,
         "TargetDBParameterGroupDescription": str,
     },
@@ -2387,20 +2448,22 @@
     "_OptionalCopyDBParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyDBParameterGroupMessageRequestTypeDef(
     _RequiredCopyDBParameterGroupMessageRequestTypeDef,
     _OptionalCopyDBParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCopyDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBSnapshotMessageRequestTypeDef",
     {
         "SourceDBSnapshotIdentifier": str,
         "TargetDBSnapshotIdentifier": str,
     },
 )
@@ -2415,19 +2478,21 @@
         "TargetCustomAvailabilityZone": str,
         "CopyOptionGroup": bool,
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class CopyDBSnapshotMessageRequestTypeDef(
     _RequiredCopyDBSnapshotMessageRequestTypeDef, _OptionalCopyDBSnapshotMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCopyOptionGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCopyOptionGroupMessageRequestTypeDef",
     {
         "SourceOptionGroupIdentifier": str,
         "TargetOptionGroupIdentifier": str,
         "TargetOptionGroupDescription": str,
     },
@@ -2436,19 +2501,21 @@
     "_OptionalCopyOptionGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyOptionGroupMessageRequestTypeDef(
     _RequiredCopyOptionGroupMessageRequestTypeDef, _OptionalCopyOptionGroupMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateBlueGreenDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBlueGreenDeploymentRequestRequestTypeDef",
     {
         "BlueGreenDeploymentName": str,
         "Source": str,
     },
 )
@@ -2459,20 +2526,22 @@
         "TargetDBParameterGroupName": str,
         "TargetDBClusterParameterGroupName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateBlueGreenDeploymentRequestRequestTypeDef(
     _RequiredCreateBlueGreenDeploymentRequestRequestTypeDef,
     _OptionalCreateBlueGreenDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateCustomDBEngineVersionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCustomDBEngineVersionMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
     },
 )
@@ -2486,20 +2555,22 @@
         "Description": str,
         "Manifest": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCustomDBEngineVersionMessageRequestTypeDef(
     _RequiredCreateCustomDBEngineVersionMessageRequestTypeDef,
     _OptionalCreateCustomDBEngineVersionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "EndpointType": str,
     },
@@ -2510,20 +2581,22 @@
         "StaticMembers": Sequence[str],
         "ExcludedMembers": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBClusterEndpointMessageRequestTypeDef(
     _RequiredCreateDBClusterEndpointMessageRequestTypeDef,
     _OptionalCreateDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
     },
@@ -2532,20 +2605,22 @@
     "_OptionalCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCreateDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterIdentifier": str,
     },
 )
@@ -2553,20 +2628,22 @@
     "_OptionalCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCreateDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCreateDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBParameterGroupMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
     },
@@ -2575,20 +2652,22 @@
     "_OptionalCreateDBParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBParameterGroupMessageRequestTypeDef(
     _RequiredCreateDBParameterGroupMessageRequestTypeDef,
     _OptionalCreateDBParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBProxyEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDBProxyEndpointRequestRequestTypeDef",
     {
         "DBProxyName": str,
         "DBProxyEndpointName": str,
         "VpcSubnetIds": Sequence[str],
     },
@@ -2599,20 +2678,22 @@
         "VpcSecurityGroupIds": Sequence[str],
         "TargetRole": DBProxyEndpointTargetRoleType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBProxyEndpointRequestRequestTypeDef(
     _RequiredCreateDBProxyEndpointRequestRequestTypeDef,
     _OptionalCreateDBProxyEndpointRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSecurityGroupMessageRequestTypeDef",
     {
         "DBSecurityGroupName": str,
         "DBSecurityGroupDescription": str,
     },
 )
@@ -2620,20 +2701,22 @@
     "_OptionalCreateDBSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBSecurityGroupMessageRequestTypeDef(
     _RequiredCreateDBSecurityGroupMessageRequestTypeDef,
     _OptionalCreateDBSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSnapshotMessageRequestTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "DBInstanceIdentifier": str,
     },
 )
@@ -2641,19 +2724,21 @@
     "_OptionalCreateDBSnapshotMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBSnapshotMessageRequestTypeDef(
     _RequiredCreateDBSnapshotMessageRequestTypeDef, _OptionalCreateDBSnapshotMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -2662,20 +2747,22 @@
     "_OptionalCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBSubnetGroupMessageRequestTypeDef(
     _RequiredCreateDBSubnetGroupMessageRequestTypeDef,
     _OptionalCreateDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "SnsTopicArn": str,
     },
 )
@@ -2687,20 +2774,22 @@
         "SourceIds": Sequence[str],
         "Enabled": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateOptionGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateOptionGroupMessageRequestTypeDef",
     {
         "OptionGroupName": str,
         "EngineName": str,
         "MajorEngineVersion": str,
         "OptionGroupDescription": str,
@@ -2710,19 +2799,21 @@
     "_OptionalCreateOptionGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateOptionGroupMessageRequestTypeDef(
     _RequiredCreateOptionGroupMessageRequestTypeDef, _OptionalCreateOptionGroupMessageRequestTypeDef
 ):
     pass
 
+
 DBClusterSnapshotTypeDef = TypedDict(
     "DBClusterSnapshotTypeDef",
     {
         "AvailabilityZones": List[str],
         "DBClusterSnapshotIdentifier": str,
         "DBClusterIdentifier": str,
         "SnapshotCreateTime": datetime,
@@ -2742,14 +2833,15 @@
         "KmsKeyId": str,
         "DBClusterSnapshotArn": str,
         "SourceDBClusterSnapshotArn": str,
         "IAMDatabaseAuthenticationEnabled": bool,
         "TagList": List[TagTypeDef],
         "DBSystemId": str,
         "StorageType": str,
+        "DbClusterResourceId": str,
     },
     total=False,
 )
 
 _RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef",
     {
@@ -2762,20 +2854,22 @@
         "ReservedDBInstanceId": str,
         "DBInstanceCount": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PurchaseReservedDBInstancesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedDBInstancesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedDBInstancesOfferingMessageRequestTypeDef,
 ):
     pass
 
+
 TagListMessageTypeDef = TypedDict(
     "TagListMessageTypeDef",
     {
         "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2834,20 +2928,22 @@
     {
         "Force": bool,
         "UseEarliestTimeOnPointInTimeUnavailable": bool,
     },
     total=False,
 )
 
+
 class BacktrackDBClusterMessageRequestTypeDef(
     _RequiredBacktrackDBClusterMessageRequestTypeDef,
     _OptionalBacktrackDBClusterMessageRequestTypeDef,
 ):
     pass
 
+
 BlueGreenDeploymentTypeDef = TypedDict(
     "BlueGreenDeploymentTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
         "BlueGreenDeploymentName": str,
         "Source": str,
         "Target": str,
@@ -2922,20 +3018,22 @@
     {
         "ConnectionPoolConfig": ConnectionPoolConfigurationTypeDef,
         "NewName": str,
     },
     total=False,
 )
 
+
 class ModifyDBProxyTargetGroupRequestRequestTypeDef(
     _RequiredModifyDBProxyTargetGroupRequestRequestTypeDef,
     _OptionalModifyDBProxyTargetGroupRequestRequestTypeDef,
 ):
     pass
 
+
 CopyDBClusterParameterGroupResultTypeDef = TypedDict(
     "CopyDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3035,24 +3133,27 @@
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
         "DBSystemId": str,
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
+        "EnableLocalWriteForwarding": bool,
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class CreateDBClusterMessageRequestTypeDef(
     _RequiredCreateDBClusterMessageRequestTypeDef, _OptionalCreateDBClusterMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalModifyDBClusterMessageRequestTypeDef = TypedDict(
@@ -3094,23 +3195,26 @@
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
         "ManageMasterUserPassword": bool,
         "RotateMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "EngineMode": str,
         "AllowEngineModeChange": bool,
+        "EnableLocalWriteForwarding": bool,
     },
     total=False,
 )
 
+
 class ModifyDBClusterMessageRequestTypeDef(
     _RequiredModifyDBClusterMessageRequestTypeDef, _OptionalModifyDBClusterMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredRestoreDBClusterFromS3MessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterFromS3MessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Engine": str,
         "MasterUsername": str,
         "SourceEngine": str,
@@ -3151,20 +3255,22 @@
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "StorageType": str,
     },
     total=False,
 )
 
+
 class RestoreDBClusterFromS3MessageRequestTypeDef(
     _RequiredRestoreDBClusterFromS3MessageRequestTypeDef,
     _OptionalRestoreDBClusterFromS3MessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "Engine": str,
     },
@@ -3197,31 +3303,33 @@
         "PubliclyAccessible": bool,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
     },
     total=False,
 )
 
+
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
-        "SourceDBClusterIdentifier": str,
     },
 )
 _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
     "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
         "RestoreType": str,
+        "SourceDBClusterIdentifier": str,
         "RestoreToTime": TimestampTypeDef,
         "UseLatestRestorableTime": bool,
         "Port": int,
         "DBSubnetGroupName": str,
         "OptionGroupName": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
@@ -3238,24 +3346,27 @@
         "EngineMode": str,
         "DBClusterInstanceClass": str,
         "StorageType": str,
         "PubliclyAccessible": bool,
         "Iops": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
         "NetworkType": str,
+        "SourceDbClusterResourceId": str,
     },
     total=False,
 )
 
+
 class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
     _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
     _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "Engine": str,
     },
@@ -3289,14 +3400,18 @@
         "DBClusterIdentifier": str,
         "StorageType": str,
         "TdeCredentialArn": str,
         "TdeCredentialPassword": str,
         "StorageEncrypted": bool,
         "KmsKeyId": str,
         "Domain": str,
+        "DomainFqdn": str,
+        "DomainOu": str,
+        "DomainAuthSecretArn": str,
+        "DomainDnsIps": Sequence[str],
         "CopyTagsToSnapshot": bool,
         "MonitoringInterval": int,
         "MonitoringRoleArn": str,
         "DomainIAMRoleName": str,
         "PromotionTier": int,
         "Timezone": str,
         "EnableIAMDatabaseAuthentication": bool,
@@ -3311,23 +3426,26 @@
         "CustomIamInstanceProfile": str,
         "BackupTarget": str,
         "NetworkType": str,
         "StorageThroughput": int,
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "CACertificateIdentifier": str,
+        "DBSystemId": str,
     },
     total=False,
 )
 
+
 class CreateDBInstanceMessageRequestTypeDef(
     _RequiredCreateDBInstanceMessageRequestTypeDef, _OptionalCreateDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalCreateDBInstanceReadReplicaMessageRequestTypeDef = TypedDict(
@@ -3358,33 +3476,39 @@
         "PerformanceInsightsRetentionPeriod": int,
         "EnableCloudwatchLogsExports": Sequence[str],
         "ProcessorFeatures": Sequence[ProcessorFeatureTypeDef],
         "UseDefaultProcessorFeatures": bool,
         "DeletionProtection": bool,
         "Domain": str,
         "DomainIAMRoleName": str,
+        "DomainFqdn": str,
+        "DomainOu": str,
+        "DomainAuthSecretArn": str,
+        "DomainDnsIps": Sequence[str],
         "ReplicaMode": ReplicaModeType,
         "MaxAllocatedStorage": int,
         "CustomIamInstanceProfile": str,
         "NetworkType": str,
         "StorageThroughput": int,
         "EnableCustomerOwnedIp": bool,
         "AllocatedStorage": int,
         "SourceDBClusterIdentifier": str,
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class CreateDBInstanceReadReplicaMessageRequestTypeDef(
     _RequiredCreateDBInstanceReadReplicaMessageRequestTypeDef,
     _OptionalCreateDBInstanceReadReplicaMessageRequestTypeDef,
 ):
     pass
 
+
 DBSnapshotTypeDef = TypedDict(
     "DBSnapshotTypeDef",
     {
         "DBSnapshotIdentifier": str,
         "DBInstanceIdentifier": str,
         "SnapshotCreateTime": datetime,
         "Engine": str,
@@ -3413,14 +3537,15 @@
         "ProcessorFeatures": List[ProcessorFeatureTypeDef],
         "DbiResourceId": str,
         "TagList": List[TagTypeDef],
         "OriginalSnapshotCreateTime": datetime,
         "SnapshotDatabaseTime": datetime,
         "SnapshotTarget": str,
         "StorageThroughput": int,
+        "DBSystemId": str,
     },
     total=False,
 )
 
 _RequiredModifyDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBInstanceMessageRequestTypeDef",
     {
@@ -3450,20 +3575,25 @@
         "OptionGroupName": str,
         "NewDBInstanceIdentifier": str,
         "StorageType": str,
         "TdeCredentialArn": str,
         "TdeCredentialPassword": str,
         "CACertificateIdentifier": str,
         "Domain": str,
+        "DomainFqdn": str,
+        "DomainOu": str,
+        "DomainAuthSecretArn": str,
+        "DomainDnsIps": Sequence[str],
         "CopyTagsToSnapshot": bool,
         "MonitoringInterval": int,
         "DBPortNumber": int,
         "PubliclyAccessible": bool,
         "MonitoringRoleArn": str,
         "DomainIAMRoleName": str,
+        "DisableDomain": bool,
         "PromotionTier": int,
         "EnableIAMDatabaseAuthentication": bool,
         "EnablePerformanceInsights": bool,
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "CloudwatchLogsExportConfiguration": CloudwatchLogsExportConfigurationTypeDef,
         "ProcessorFeatures": Sequence[ProcessorFeatureTypeDef],
@@ -3482,19 +3612,21 @@
         "RotateMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
         "Engine": str,
     },
     total=False,
 )
 
+
 class ModifyDBInstanceMessageRequestTypeDef(
     _RequiredModifyDBInstanceMessageRequestTypeDef, _OptionalModifyDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 PendingModifiedValuesTypeDef = TypedDict(
     "PendingModifiedValuesTypeDef",
     {
         "DBInstanceClass": str,
         "AllocatedStorage": int,
         "MasterUserPassword": str,
         "Port": int,
@@ -3542,14 +3674,18 @@
         "OptionGroupName": str,
         "Tags": Sequence[TagTypeDef],
         "StorageType": str,
         "TdeCredentialArn": str,
         "TdeCredentialPassword": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Domain": str,
+        "DomainFqdn": str,
+        "DomainOu": str,
+        "DomainAuthSecretArn": str,
+        "DomainDnsIps": Sequence[str],
         "CopyTagsToSnapshot": bool,
         "DomainIAMRoleName": str,
         "EnableIAMDatabaseAuthentication": bool,
         "EnableCloudwatchLogsExports": Sequence[str],
         "ProcessorFeatures": Sequence[ProcessorFeatureTypeDef],
         "UseDefaultProcessorFeatures": bool,
         "DBParameterGroupName": str,
@@ -3561,20 +3697,22 @@
         "StorageThroughput": int,
         "DBClusterSnapshotIdentifier": str,
         "AllocatedStorage": int,
     },
     total=False,
 )
 
+
 class RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBInstanceFromDBSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreDBInstanceFromS3MessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceFromS3MessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "Engine": str,
         "SourceEngine": str,
@@ -3627,20 +3765,22 @@
         "StorageThroughput": int,
         "ManageMasterUserPassword": bool,
         "MasterUserSecretKmsKeyId": str,
     },
     total=False,
 )
 
+
 class RestoreDBInstanceFromS3MessageRequestTypeDef(
     _RequiredRestoreDBInstanceFromS3MessageRequestTypeDef,
     _OptionalRestoreDBInstanceFromS3MessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     {
         "TargetDBInstanceIdentifier": str,
     },
 )
 _OptionalRestoreDBInstanceToPointInTimeMessageRequestTypeDef = TypedDict(
@@ -3665,14 +3805,18 @@
         "Tags": Sequence[TagTypeDef],
         "StorageType": str,
         "TdeCredentialArn": str,
         "TdeCredentialPassword": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Domain": str,
         "DomainIAMRoleName": str,
+        "DomainFqdn": str,
+        "DomainOu": str,
+        "DomainAuthSecretArn": str,
+        "DomainDnsIps": Sequence[str],
         "EnableIAMDatabaseAuthentication": bool,
         "EnableCloudwatchLogsExports": Sequence[str],
         "ProcessorFeatures": Sequence[ProcessorFeatureTypeDef],
         "UseDefaultProcessorFeatures": bool,
         "DBParameterGroupName": str,
         "DeletionProtection": bool,
         "SourceDbiResourceId": str,
@@ -3684,20 +3828,22 @@
         "NetworkType": str,
         "StorageThroughput": int,
         "AllocatedStorage": int,
     },
     total=False,
 )
 
+
 class RestoreDBInstanceToPointInTimeMessageRequestTypeDef(
     _RequiredRestoreDBInstanceToPointInTimeMessageRequestTypeDef,
     _OptionalRestoreDBInstanceToPointInTimeMessageRequestTypeDef,
 ):
     pass
 
+
 CreateDBProxyEndpointResponseTypeDef = TypedDict(
     "CreateDBProxyEndpointResponseTypeDef",
     {
         "DBProxyEndpoint": DBProxyEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3745,19 +3891,21 @@
         "IdleClientTimeout": int,
         "DebugLogging": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBProxyRequestRequestTypeDef(
     _RequiredCreateDBProxyRequestRequestTypeDef, _OptionalCreateDBProxyRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyDBProxyRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDBProxyRequestRequestTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalModifyDBProxyRequestRequestTypeDef = TypedDict(
@@ -3770,19 +3918,51 @@
         "DebugLogging": bool,
         "RoleArn": str,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyDBProxyRequestRequestTypeDef(
     _RequiredModifyDBProxyRequestRequestTypeDef, _OptionalModifyDBProxyRequestRequestTypeDef
 ):
     pass
 
+
+DBClusterAutomatedBackupTypeDef = TypedDict(
+    "DBClusterAutomatedBackupTypeDef",
+    {
+        "Engine": str,
+        "VpcId": str,
+        "DBClusterAutomatedBackupsArn": str,
+        "DBClusterIdentifier": str,
+        "RestoreWindow": RestoreWindowTypeDef,
+        "MasterUsername": str,
+        "DbClusterResourceId": str,
+        "Region": str,
+        "LicenseModel": str,
+        "Status": str,
+        "IAMDatabaseAuthenticationEnabled": bool,
+        "ClusterCreateTime": datetime,
+        "StorageEncrypted": bool,
+        "AllocatedStorage": int,
+        "EngineVersion": str,
+        "DBClusterArn": str,
+        "BackupRetentionPeriod": int,
+        "EngineMode": str,
+        "AvailabilityZones": List[str],
+        "Port": int,
+        "KmsKeyId": str,
+        "StorageType": str,
+        "Iops": int,
+    },
+    total=False,
+)
+
 DBClusterBacktrackMessageTypeDef = TypedDict(
     "DBClusterBacktrackMessageTypeDef",
     {
         "Marker": str,
         "DBClusterBacktracks": List[DBClusterBacktrackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3796,39 +3976,101 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBParameterGroupDetailsTypeDef = TypedDict(
     "DBParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
+    },
+    total=False,
+)
+
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+
+_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+    },
+)
+_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
     },
     total=False,
 )
 
+
+class ResetDBParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
     total=False,
@@ -3864,14 +4106,15 @@
         "KMSKeyId": str,
         "CreateTime": datetime,
         "TagList": List[TagTypeDef],
         "SupportsBabelfish": bool,
         "CustomDBEngineVersionManifest": str,
         "SupportsCertificateRotationWithoutRestart": bool,
         "SupportedCACertificateIdentifiers": List[str],
+        "SupportsLocalWriteForwarding": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBEngineVersionTypeDef = TypedDict(
     "DBEngineVersionTypeDef",
     {
@@ -3902,14 +4145,15 @@
         "KMSKeyId": str,
         "CreateTime": datetime,
         "TagList": List[TagTypeDef],
         "SupportsBabelfish": bool,
         "CustomDBEngineVersionManifest": str,
         "SupportsCertificateRotationWithoutRestart": bool,
         "SupportedCACertificateIdentifiers": List[str],
+        "SupportsLocalWriteForwarding": bool,
     },
     total=False,
 )
 
 DBInstanceAutomatedBackupTypeDef = TypedDict(
     "DBInstanceAutomatedBackupTypeDef",
     {
@@ -4025,14 +4269,26 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeDBClusterAutomatedBackupsMessageRequestTypeDef = TypedDict(
+    "DescribeDBClusterAutomatedBackupsMessageRequestTypeDef",
+    {
+        "DbClusterResourceId": str,
+        "DBClusterIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
 _RequiredDescribeDBClusterBacktracksMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBClusterBacktracksMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalDescribeDBClusterBacktracksMessageRequestTypeDef = TypedDict(
@@ -4042,20 +4298,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeDBClusterBacktracksMessageRequestTypeDef(
     _RequiredDescribeDBClusterBacktracksMessageRequestTypeDef,
     _OptionalDescribeDBClusterBacktracksMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeDBClusterEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
@@ -4088,31 +4346,34 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeDBClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDBClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDBClusterParametersMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeDBClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
+        "DbClusterResourceId": str,
     },
     total=False,
 )
 
 DescribeDBClustersMessageRequestTypeDef = TypedDict(
     "DescribeDBClustersMessageRequestTypeDef",
     {
@@ -4181,20 +4442,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeDBLogFilesMessageRequestTypeDef(
     _RequiredDescribeDBLogFilesMessageRequestTypeDef,
     _OptionalDescribeDBLogFilesMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeDBParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBParameterGroupsMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -4215,20 +4478,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeDBParametersMessageRequestTypeDef(
     _RequiredDescribeDBParametersMessageRequestTypeDef,
     _OptionalDescribeDBParametersMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeDBProxiesRequestRequestTypeDef = TypedDict(
     "DescribeDBProxiesRequestRequestTypeDef",
     {
         "DBProxyName": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4261,20 +4526,22 @@
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+
 class DescribeDBProxyTargetGroupsRequestRequestTypeDef(
     _RequiredDescribeDBProxyTargetGroupsRequestRequestTypeDef,
     _OptionalDescribeDBProxyTargetGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeDBProxyTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDBProxyTargetsRequestRequestTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalDescribeDBProxyTargetsRequestRequestTypeDef = TypedDict(
@@ -4284,20 +4551,22 @@
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+
 class DescribeDBProxyTargetsRequestRequestTypeDef(
     _RequiredDescribeDBProxyTargetsRequestRequestTypeDef,
     _OptionalDescribeDBProxyTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeDBSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBSecurityGroupsMessageRequestTypeDef",
     {
         "DBSecurityGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -4344,20 +4613,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
         "DBParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -4366,20 +4637,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeEventCategoriesMessageRequestTypeDef = TypedDict(
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
@@ -4449,20 +4722,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeOptionGroupOptionsMessageRequestTypeDef(
     _RequiredDescribeOptionGroupOptionsMessageRequestTypeDef,
     _OptionalDescribeOptionGroupOptionsMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeOptionGroupsMessageRequestTypeDef = TypedDict(
     "DescribeOptionGroupsMessageRequestTypeDef",
     {
         "OptionGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4489,20 +4764,22 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
 ):
     pass
 
+
 DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -4565,20 +4842,22 @@
     "_OptionalListTagsForResourceMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+
 class ListTagsForResourceMessageRequestTypeDef(
     _RequiredListTagsForResourceMessageRequestTypeDef,
     _OptionalListTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeBlueGreenDeploymentsRequestDescribeBlueGreenDeploymentsPaginateTypeDef = TypedDict(
     "DescribeBlueGreenDeploymentsRequestDescribeBlueGreenDeploymentsPaginateTypeDef",
     {
         "BlueGreenDeploymentIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4607,20 +4886,22 @@
         "BacktrackIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef(
     _RequiredDescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef,
     _OptionalDescribeDBClusterBacktracksMessageDescribeDBClusterBacktracksPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -4650,29 +4931,32 @@
         "Source": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
     _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "IncludeShared": bool,
         "IncludePublic": bool,
+        "DbClusterResourceId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
     "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
@@ -4737,20 +5021,22 @@
         "FileSize": int,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef(
     _RequiredDescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef,
     _OptionalDescribeDBLogFilesMessageDescribeDBLogFilesPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
     "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     {
         "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4769,20 +5055,22 @@
         "Source": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
     _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBProxiesRequestDescribeDBProxiesPaginateTypeDef = TypedDict(
     "DescribeDBProxiesRequestDescribeDBProxiesPaginateTypeDef",
     {
         "DBProxyName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4812,20 +5100,22 @@
         "TargetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef(
     _RequiredDescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef,
     _OptionalDescribeDBProxyTargetGroupsRequestDescribeDBProxyTargetGroupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef",
     {
         "DBProxyName": str,
     },
 )
 _OptionalDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef = TypedDict(
@@ -4834,20 +5124,22 @@
         "TargetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef(
     _RequiredDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef,
     _OptionalDescribeDBProxyTargetsRequestDescribeDBProxyTargetsPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBSecurityGroupsMessageDescribeDBSecurityGroupsPaginateTypeDef = TypedDict(
     "DescribeDBSecurityGroupsMessageDescribeDBSecurityGroupsPaginateTypeDef",
     {
         "DBSecurityGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4890,20 +5182,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageDescribeEngineDefaultClusterParametersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     {
         "DBParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
@@ -4911,20 +5205,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
 ):
     pass
 
+
 DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -4980,20 +5276,22 @@
         "MajorEngineVersion": str,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef(
     _RequiredDescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef,
     _OptionalDescribeOptionGroupOptionsMessageDescribeOptionGroupOptionsPaginateTypeDef,
 ):
     pass
 
+
 DescribeOptionGroupsMessageDescribeOptionGroupsPaginateTypeDef = TypedDict(
     "DescribeOptionGroupsMessageDescribeOptionGroupsPaginateTypeDef",
     {
         "OptionGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "EngineName": str,
         "MajorEngineVersion": str,
@@ -5018,20 +5316,22 @@
         "Vpc": bool,
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
 ):
     pass
 
+
 DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
     TypedDict(
         "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
         {
             "ResourceIdentifier": str,
             "Filters": Sequence[FilterTypeDef],
             "PaginationConfig": PaginatorConfigTypeDef,
@@ -5093,31 +5393,34 @@
     "_OptionalDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef(
     _RequiredDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef,
     _OptionalDownloadDBLogFilePortionMessageDownloadDBLogFilePortionPaginateTypeDef,
 ):
     pass
 
+
 DescribeDBClusterSnapshotsMessageDBClusterSnapshotAvailableWaitTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDBClusterSnapshotAvailableWaitTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
+        "DbClusterResourceId": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClusterSnapshotsMessageDBClusterSnapshotDeletedWaitTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageDBClusterSnapshotDeletedWaitTypeDef",
@@ -5126,14 +5429,15 @@
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
+        "DbClusterResourceId": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDBClustersMessageDBClusterAvailableWaitTypeDef = TypedDict(
     "DescribeDBClustersMessageDBClusterAvailableWaitTypeDef",
@@ -5318,19 +5622,21 @@
         "DBSecurityGroupMemberships": Sequence[str],
         "VpcSecurityGroupMemberships": Sequence[str],
         "OptionSettings": Sequence[OptionSettingTypeDef],
     },
     total=False,
 )
 
+
 class OptionConfigurationTypeDef(
     _RequiredOptionConfigurationTypeDef, _OptionalOptionConfigurationTypeDef
 ):
     pass
 
+
 OptionTypeDef = TypedDict(
     "OptionTypeDef",
     {
         "OptionName": str,
         "OptionDescription": str,
         "Persistent": bool,
         "Permanent": bool,
@@ -5350,15 +5656,14 @@
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetOutpost": OutpostTypeDef,
         "SubnetStatus": str,
     },
     total=False,
 )
 
-ParameterUnionTypeDef = Union[ParameterTypeDef, ParameterOutputTypeDef]
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -5573,14 +5878,15 @@
         "PerformanceInsightsKMSKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationInfoTypeDef,
         "NetworkType": str,
         "DBSystemId": str,
         "MasterUserSecret": MasterUserSecretTypeDef,
         "IOOptimizedNextAllowedModificationTime": datetime,
+        "LocalWriteForwardingStatus": LocalWriteForwardingStatusType,
     },
     total=False,
 )
 
 DescribeDBProxyTargetGroupsResponseTypeDef = TypedDict(
     "DescribeDBProxyTargetGroupsResponseTypeDef",
     {
@@ -5635,14 +5941,31 @@
     "ModifyDBSnapshotResultTypeDef",
     {
         "DBSnapshot": DBSnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DBClusterAutomatedBackupMessageTypeDef = TypedDict(
+    "DBClusterAutomatedBackupMessageTypeDef",
+    {
+        "Marker": str,
+        "DBClusterAutomatedBackups": List[DBClusterAutomatedBackupTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDBClusterAutomatedBackupResultTypeDef = TypedDict(
+    "DeleteDBClusterAutomatedBackupResultTypeDef",
+    {
+        "DBClusterAutomatedBackup": DBClusterAutomatedBackupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5897,19 +6220,21 @@
         "OptionsToInclude": Sequence[OptionConfigurationTypeDef],
         "OptionsToRemove": Sequence[str],
         "ApplyImmediately": bool,
     },
     total=False,
 )
 
+
 class ModifyOptionGroupMessageRequestTypeDef(
     _RequiredModifyOptionGroupMessageRequestTypeDef, _OptionalModifyOptionGroupMessageRequestTypeDef
 ):
     pass
 
+
 OptionGroupTypeDef = TypedDict(
     "OptionGroupTypeDef",
     {
         "OptionGroupName": str,
         "OptionGroupDescription": str,
         "EngineName": str,
         "MajorEngineVersion": str,
@@ -5934,72 +6259,14 @@
         "Subnets": List[SubnetTypeDef],
         "DBSubnetGroupArn": str,
         "SupportedNetworkTypes": List[str],
     },
     total=False,
 )
 
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-)
-
-ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-)
-
-_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-    total=False,
-)
-
-class ResetDBClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
-
-_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-    },
-)
-_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterUnionTypeDef],
-    },
-    total=False,
-)
-
-class ResetDBParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBParameterGroupMessageRequestTypeDef,
-):
-    pass
-
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6277,14 +6544,15 @@
         "NetworkType": str,
         "ActivityStreamPolicyStatus": ActivityStreamPolicyStatusType,
         "StorageThroughput": int,
         "DBSystemId": str,
         "MasterUserSecret": MasterUserSecretTypeDef,
         "CertificateDetails": CertificateDetailsTypeDef,
         "ReadReplicaSourceDBClusterIdentifier": str,
+        "PercentProgress": str,
     },
     total=False,
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
```

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/waiter.py` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
+        DbClusterResourceId: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotavailablewaiter)
         """
 
@@ -137,14 +138,15 @@
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
+        DbClusterResourceId: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotdeletedwaiter)
         """
```

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds/waiter.pyi` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds/waiter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
+        DbClusterResourceId: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotavailablewaiter)
         """
 
@@ -133,14 +134,15 @@
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
+        DbClusterResourceId: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Waiter.DBClusterSnapshotDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/waiters/#dbclustersnapshotdeletedwaiter)
         """
```

### Comparing `types-aiobotocore-rds-2.5.2.post1/types_aiobotocore_rds.egg-info/SOURCES.txt` & `types-aiobotocore-rds-2.5.2.post2/types_aiobotocore_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

