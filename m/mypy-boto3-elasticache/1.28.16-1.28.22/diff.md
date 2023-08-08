# Comparing `tmp/mypy-boto3-elasticache-1.28.16.tar.gz` & `tmp/mypy-boto3-elasticache-1.28.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticache-1.28.16.tar", last modified: Tue Aug  1 11:36:42 2023, max compression
+gzip compressed data, was "mypy-boto3-elasticache-1.28.22.tar", last modified: Tue Aug  8 19:32:24 2023, max compression
```

## Comparing `mypy-boto3-elasticache-1.28.16.tar` & `mypy-boto3-elasticache-1.28.22.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.916900 mypy-boto3-elasticache-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27341 2023-08-01 11:36:42.912900 mypy-boto3-elasticache-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25841 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.900900 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67982 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    67889 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-08-01 11:17:13.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-08-01 11:17:13.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22637 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22618 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86817 2023-08-01 11:17:16.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86750 2023-08-01 11:17:14.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-08-01 11:17:12.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.912900 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27341 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:36:42.000000 mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:42.916900 mypy-boto3-elasticache-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-01 11:17:11.000000 mypy-boto3-elasticache-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:32:24.889480 mypy-boto3-elasticache-1.28.22/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 19:32:06.000000 mypy-boto3-elasticache-1.28.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-08-08 19:32:24.889480 mypy-boto3-elasticache-1.28.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-08-08 19:32:06.000000 mypy-boto3-elasticache-1.28.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:32:24.885480 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-08 19:32:06.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-08-08 19:32:06.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-08 19:32:06.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68600 2023-08-08 19:32:07.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68506 2023-08-08 19:32:07.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-08-08 19:32:07.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-08-08 19:32:07.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22637 2023-08-08 19:32:07.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22618 2023-08-08 19:32:07.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:32:06.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86724 2023-08-08 19:32:10.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86657 2023-08-08 19:32:09.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-08 19:32:06.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-08-08 19:32:07.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-08-08 19:32:07.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:32:24.889480 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-08-08 19:32:24.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-08 19:32:24.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:32:24.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:32:24.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 19:32:24.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 19:32:24.000000 mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 19:32:24.889480 mypy-boto3-elasticache-1.28.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-08 19:32:06.000000 mypy-boto3-elasticache-1.28.22/setup.py
```

### Comparing `mypy-boto3-elasticache-1.28.16/LICENSE` & `mypy-boto3-elasticache-1.28.22/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__init__.py` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__init__.pyi` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/__main__.py` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElastiCache 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for boto3.ElastiCache 1.28.22\nVersion:         1.28.22\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.22")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/client.py` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     IncreaseReplicaCountResultTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     ModifyCacheClusterResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     ModifyReplicationGroupResultTypeDef,
     ModifyReplicationGroupShardConfigurationResultTypeDef,
-    NodeGroupConfigurationUnionTypeDef,
+    NodeGroupConfigurationTypeDef,
     ParameterNameValueTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     RebootCacheClusterResultTypeDef,
     RegionalConfigurationTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
@@ -107,14 +107,15 @@
     ReshardingConfigurationTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
     ServiceUpdatesMessageTypeDef,
     StartMigrationResponseTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
     TestFailoverResultTypeDef,
+    TestMigrationResponseTypeDef,
     TimeRangeFilterTypeDef,
     TimestampTypeDef,
     UpdateActionResultsMessageTypeDef,
     UpdateActionsMessageTypeDef,
     UserGroupResponseTypeDef,
     UserResponseTypeDef,
 )
@@ -429,15 +430,15 @@
         PrimaryClusterId: str = ...,
         AutomaticFailoverEnabled: bool = ...,
         MultiAZEnabled: bool = ...,
         NumCacheClusters: int = ...,
         PreferredCacheClusterAZs: Sequence[str] = ...,
         NumNodeGroups: int = ...,
         ReplicasPerNodeGroup: int = ...,
-        NodeGroupConfiguration: Sequence[NodeGroupConfigurationUnionTypeDef] = ...,
+        NodeGroupConfiguration: Sequence[NodeGroupConfigurationTypeDef] = ...,
         CacheNodeType: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         CacheSubnetGroupName: str = ...,
         CacheSecurityGroupNames: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
@@ -1250,14 +1251,27 @@
         on a specified node group (called shard in the console) in a replication group
         (called cluster in the console).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.test_failover)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#test_failover)
         """
 
+    def test_migration(
+        self,
+        *,
+        ReplicationGroupId: str,
+        CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef]
+    ) -> TestMigrationResponseTypeDef:
+        """
+        Async API to test connection between source and target replication group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.test_migration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#test_migration)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cache_clusters"]
     ) -> DescribeCacheClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#get_paginator)
```

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/client.pyi` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     IncreaseReplicaCountResultTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     ModifyCacheClusterResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     ModifyReplicationGroupResultTypeDef,
     ModifyReplicationGroupShardConfigurationResultTypeDef,
-    NodeGroupConfigurationUnionTypeDef,
+    NodeGroupConfigurationTypeDef,
     ParameterNameValueTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     RebootCacheClusterResultTypeDef,
     RegionalConfigurationTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
@@ -107,14 +107,15 @@
     ReshardingConfigurationTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
     ServiceUpdatesMessageTypeDef,
     StartMigrationResponseTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
     TestFailoverResultTypeDef,
+    TestMigrationResponseTypeDef,
     TimeRangeFilterTypeDef,
     TimestampTypeDef,
     UpdateActionResultsMessageTypeDef,
     UpdateActionsMessageTypeDef,
     UserGroupResponseTypeDef,
     UserResponseTypeDef,
 )
@@ -411,15 +412,15 @@
         PrimaryClusterId: str = ...,
         AutomaticFailoverEnabled: bool = ...,
         MultiAZEnabled: bool = ...,
         NumCacheClusters: int = ...,
         PreferredCacheClusterAZs: Sequence[str] = ...,
         NumNodeGroups: int = ...,
         ReplicasPerNodeGroup: int = ...,
-        NodeGroupConfiguration: Sequence[NodeGroupConfigurationUnionTypeDef] = ...,
+        NodeGroupConfiguration: Sequence[NodeGroupConfigurationTypeDef] = ...,
         CacheNodeType: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         CacheSubnetGroupName: str = ...,
         CacheSecurityGroupNames: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
@@ -1177,14 +1178,26 @@
         Represents the input of a `TestFailover` operation which test automatic failover
         on a specified node group (called shard in the console) in a replication group
         (called cluster in the console).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.test_failover)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#test_failover)
         """
+    def test_migration(
+        self,
+        *,
+        ReplicationGroupId: str,
+        CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef]
+    ) -> TestMigrationResponseTypeDef:
+        """
+        Async API to test connection between source and target replication group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.test_migration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#test_migration)
+        """
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cache_clusters"]
     ) -> DescribeCacheClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/client/#get_paginator)
```

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/literals.py` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,14 +559,15 @@
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

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/literals.pyi` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -557,14 +557,15 @@
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

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/paginator.py` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/paginator.pyi` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/type_defs.py` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     "ParameterTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteCacheClusterMessageRequestTypeDef",
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     "DeleteCacheSecurityGroupMessageRequestTypeDef",
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
@@ -117,16 +118,14 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
-    "NodeGroupConfigurationOutputTypeDef",
-    "NodeGroupConfigurationTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
@@ -158,15 +157,17 @@
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
+    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
+    "TestMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
     "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
@@ -189,16 +190,14 @@
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
-    "NodeSnapshotTypeDef",
-    "NodeGroupConfigurationUnionTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
     "UpdateActionResultsMessageTypeDef",
@@ -208,14 +207,15 @@
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
+    "SnapshotTypeDef",
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     "DescribeUpdateActionsMessageRequestTypeDef",
     "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
@@ -223,32 +223,31 @@
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
-    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReplicationGroupPendingModifiedValuesTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -262,14 +261,15 @@
     "DeleteReplicationGroupResultTypeDef",
     "IncreaseReplicaCountResultTypeDef",
     "ModifyReplicationGroupResultTypeDef",
     "ModifyReplicationGroupShardConfigurationResultTypeDef",
     "ReplicationGroupMessageTypeDef",
     "StartMigrationResponseTypeDef",
     "TestFailoverResultTypeDef",
+    "TestMigrationResponseTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -558,14 +558,28 @@
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
+NodeGroupConfigurationTypeDef = TypedDict(
+    "NodeGroupConfigurationTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
 CustomerNodeEndpointTypeDef = TypedDict(
     "CustomerNodeEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
     },
     total=False,
@@ -1075,42 +1089,14 @@
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
 
-NodeGroupConfigurationOutputTypeDef = TypedDict(
-    "NodeGroupConfigurationOutputTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
-    },
-    total=False,
-)
-
-NodeGroupConfigurationTypeDef = TypedDict(
-    "NodeGroupConfigurationTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": Sequence[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": Sequence[str],
-    },
-    total=False,
-)
-
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1666,22 +1652,44 @@
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
 
+TestMigrationMessageRequestTypeDef = TypedDict(
+    "TestMigrationMessageRequestTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
+    },
+)
+
 DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef = TypedDict(
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     {
         "CacheClusterId": str,
         "MaxRecords": int,
         "Marker": str,
         "ShowCacheNodeInfo": bool,
@@ -2058,31 +2066,14 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
-NodeGroupConfigurationUnionTypeDef = Union[
-    NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef
-]
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2262,14 +2253,49 @@
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
         "ServiceUpdateName": str,
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
         "Engine": str,
@@ -2428,49 +2454,14 @@
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
-    {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
-        "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
-    },
-    total=False,
-)
-
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2543,14 +2534,47 @@
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalCreateCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2611,15 +2635,15 @@
         "PrimaryClusterId": str,
         "AutomaticFailoverEnabled": bool,
         "MultiAZEnabled": bool,
         "NumCacheClusters": int,
         "PreferredCacheClusterAZs": Sequence[str],
         "NumNodeGroups": int,
         "ReplicasPerNodeGroup": int,
-        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationUnionTypeDef],
+        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationTypeDef],
         "CacheNodeType": str,
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupName": str,
         "CacheSubnetGroupName": str,
         "CacheSecurityGroupNames": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -2772,47 +2796,14 @@
         "TransitEncryptionEnabled": bool,
         "TransitEncryptionMode": TransitEncryptionModeType,
         "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
-    {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3038,7 +3029,15 @@
 TestFailoverResultTypeDef = TypedDict(
     "TestFailoverResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+TestMigrationResponseTypeDef = TypedDict(
+    "TestMigrationResponseTypeDef",
+    {
+        "ReplicationGroup": ReplicationGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/type_defs.pyi` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "ParameterTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteCacheClusterMessageRequestTypeDef",
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     "DeleteCacheSecurityGroupMessageRequestTypeDef",
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
@@ -116,16 +117,14 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
-    "NodeGroupConfigurationOutputTypeDef",
-    "NodeGroupConfigurationTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
@@ -157,15 +156,17 @@
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
+    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
+    "TestMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
     "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
@@ -188,16 +189,14 @@
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
-    "NodeSnapshotTypeDef",
-    "NodeGroupConfigurationUnionTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
     "UpdateActionResultsMessageTypeDef",
@@ -207,14 +206,15 @@
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
+    "SnapshotTypeDef",
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     "DescribeUpdateActionsMessageRequestTypeDef",
     "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
@@ -222,32 +222,31 @@
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
-    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReplicationGroupPendingModifiedValuesTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -261,14 +260,15 @@
     "DeleteReplicationGroupResultTypeDef",
     "IncreaseReplicaCountResultTypeDef",
     "ModifyReplicationGroupResultTypeDef",
     "ModifyReplicationGroupShardConfigurationResultTypeDef",
     "ReplicationGroupMessageTypeDef",
     "StartMigrationResponseTypeDef",
     "TestFailoverResultTypeDef",
+    "TestMigrationResponseTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -547,14 +547,28 @@
 
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+NodeGroupConfigurationTypeDef = TypedDict(
+    "NodeGroupConfigurationTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
 CustomerNodeEndpointTypeDef = TypedDict(
     "CustomerNodeEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
     },
     total=False,
@@ -1048,42 +1062,14 @@
 )
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
-NodeGroupConfigurationOutputTypeDef = TypedDict(
-    "NodeGroupConfigurationOutputTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
-    },
-    total=False,
-)
-
-NodeGroupConfigurationTypeDef = TypedDict(
-    "NodeGroupConfigurationTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": Sequence[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": Sequence[str],
-    },
-    total=False,
-)
-
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1617,22 +1603,44 @@
 
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
 
+TestMigrationMessageRequestTypeDef = TypedDict(
+    "TestMigrationMessageRequestTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
+    },
+)
+
 DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef = TypedDict(
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     {
         "CacheClusterId": str,
         "MaxRecords": int,
         "Marker": str,
         "ShowCacheNodeInfo": bool,
@@ -2001,31 +2009,14 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
-NodeGroupConfigurationUnionTypeDef = Union[
-    NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef
-]
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2205,14 +2196,49 @@
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
         "ServiceUpdateName": str,
         "ReplicationGroupIds": Sequence[str],
         "CacheClusterIds": Sequence[str],
         "Engine": str,
@@ -2369,49 +2395,14 @@
 
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
-    {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
-        "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
-    },
-    total=False,
-)
-
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2484,14 +2475,47 @@
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
 )
 _OptionalCreateCacheClusterMessageRequestTypeDef = TypedDict(
@@ -2550,15 +2574,15 @@
         "PrimaryClusterId": str,
         "AutomaticFailoverEnabled": bool,
         "MultiAZEnabled": bool,
         "NumCacheClusters": int,
         "PreferredCacheClusterAZs": Sequence[str],
         "NumNodeGroups": int,
         "ReplicasPerNodeGroup": int,
-        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationUnionTypeDef],
+        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationTypeDef],
         "CacheNodeType": str,
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupName": str,
         "CacheSubnetGroupName": str,
         "CacheSecurityGroupNames": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -2705,47 +2729,14 @@
         "TransitEncryptionEnabled": bool,
         "TransitEncryptionMode": TransitEncryptionModeType,
         "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
-    {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2971,7 +2962,15 @@
 TestFailoverResultTypeDef = TypedDict(
     "TestFailoverResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+TestMigrationResponseTypeDef = TypedDict(
+    "TestMigrationResponseTypeDef",
+    {
+        "ReplicationGroup": ReplicationGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/waiter.py` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache/waiter.pyi` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.16/mypy_boto3_elasticache.egg-info/SOURCES.txt` & `mypy-boto3-elasticache-1.28.22/mypy_boto3_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.16/setup.py` & `mypy-boto3-elasticache-1.28.22/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elasticache",
-    version="1.28.16",
+    version="1.28.22",
     packages=["mypy_boto3_elasticache"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElastiCache 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.ElastiCache 1.28.22 service generated with mypy-boto3-builder"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

