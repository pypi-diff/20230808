# Comparing `tmp/types-aiobotocore-eks-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-eks-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-eks-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-eks-2.5.4.tar", last modified: Tue Aug  8 01:23:40 2023, max compression
```

## Comparing `types-aiobotocore-eks-2.5.2.post3.tar` & `types-aiobotocore-eks-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.499712 types-aiobotocore-eks-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:23:05.000000 types-aiobotocore-eks-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-08-04 12:37:39.499712 types-aiobotocore-eks-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-08-04 12:23:05.000000 types-aiobotocore-eks-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:39.499712 types-aiobotocore-eks-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:23:05.000000 types-aiobotocore-eks-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.495712 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-04 12:23:05.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-08-04 12:23:05.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:23:05.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-08-04 12:23:06.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35095 2023-08-04 12:23:06.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-08-04 12:23:06.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-08-04 12:23:06.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-04 12:23:06.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-08-04 12:23:06.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:23:05.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50618 2023-08-04 12:23:08.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50545 2023-08-04 12:23:08.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:23:05.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-08-04 12:23:06.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-04 12:23:06.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.499712 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-08-04 12:37:39.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:37:39.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:39.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:39.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:39.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:39.000000 types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.802704 types-aiobotocore-eks-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-08-08 01:23:40.798704 types-aiobotocore-eks-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:40.802704 types-aiobotocore-eks-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.798704 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35095 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-08-08 01:10:33.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50618 2023-08-08 01:10:35.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50545 2023-08-08 01:10:34.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-08 01:10:32.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:40.798704 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-08-08 01:23:40.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 01:23:40.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:40.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:40.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:40.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:40.000000 types-aiobotocore-eks-2.5.4/types_aiobotocore_eks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-eks-2.5.2.post3/LICENSE` & `types-aiobotocore-eks-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post3/PKG-INFO` & `types-aiobotocore-eks-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-eks
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EKS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EKS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-eks)](https://pepy.tech/project/types-aiobotocore-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EKS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[aiobotocore.EKS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-eks-2.5.2.post3/README.md` & `types-aiobotocore-eks-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-eks)](https://pepy.tech/project/types-aiobotocore-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EKS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[aiobotocore.EKS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-eks-2.5.2.post3/setup.py` & `types-aiobotocore-eks-2.5.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-eks",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_eks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EKS 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.EKS 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/__init__.py` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/__init__.pyi` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/client.py` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/client.pyi` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/literals.py` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,32 +147,46 @@
 ListNodegroupsPaginatorName = Literal["list_nodegroups"]
 ListUpdatesPaginatorName = Literal["list_updates"]
 LogTypeType = Literal["api", "audit", "authenticator", "controllerManager", "scheduler"]
 NodegroupActiveWaiterName = Literal["nodegroup_active"]
 NodegroupDeletedWaiterName = Literal["nodegroup_deleted"]
 NodegroupIssueCodeType = Literal[
     "AccessDenied",
+    "AmiIdNotFound",
     "AsgInstanceLaunchFailures",
+    "AutoScalingGroupInstanceRefreshActive",
     "AutoScalingGroupInvalidConfiguration",
     "AutoScalingGroupNotFound",
+    "AutoScalingGroupOptInRequired",
+    "AutoScalingGroupRateLimitExceeded",
     "ClusterUnreachable",
+    "Ec2LaunchTemplateDeletionFailure",
+    "Ec2LaunchTemplateInvalidConfiguration",
+    "Ec2LaunchTemplateMaxLimitExceeded",
     "Ec2LaunchTemplateNotFound",
     "Ec2LaunchTemplateVersionMismatch",
     "Ec2SecurityGroupDeletionFailure",
     "Ec2SecurityGroupNotFound",
     "Ec2SubnetInvalidConfiguration",
+    "Ec2SubnetListTooLong",
     "Ec2SubnetMissingIpv6Assignment",
     "Ec2SubnetNotFound",
     "IamInstanceProfileNotFound",
     "IamLimitExceeded",
     "IamNodeRoleNotFound",
+    "IamThrottling",
     "InstanceLimitExceeded",
     "InsufficientFreeAddresses",
     "InternalFailure",
+    "LimitExceeded",
     "NodeCreationFailure",
+    "NodeTerminationFailure",
+    "PodEvictionFailure",
+    "SourceEc2LaunchTemplateNotFound",
+    "Unknown",
 ]
 NodegroupStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATING", "DEGRADED", "DELETE_FAILED", "DELETING", "UPDATING"
 ]
 ResolveConflictsType = Literal["NONE", "OVERWRITE", "PRESERVE"]
 TaintEffectType = Literal["NO_EXECUTE", "NO_SCHEDULE", "PREFER_NO_SCHEDULE"]
 UpdateParamTypeType = Literal[
@@ -224,14 +238,15 @@
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
@@ -327,14 +342,15 @@
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
@@ -413,26 +429,28 @@
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
@@ -612,14 +630,15 @@
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

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/literals.pyi` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -145,32 +145,46 @@
 ListNodegroupsPaginatorName = Literal["list_nodegroups"]
 ListUpdatesPaginatorName = Literal["list_updates"]
 LogTypeType = Literal["api", "audit", "authenticator", "controllerManager", "scheduler"]
 NodegroupActiveWaiterName = Literal["nodegroup_active"]
 NodegroupDeletedWaiterName = Literal["nodegroup_deleted"]
 NodegroupIssueCodeType = Literal[
     "AccessDenied",
+    "AmiIdNotFound",
     "AsgInstanceLaunchFailures",
+    "AutoScalingGroupInstanceRefreshActive",
     "AutoScalingGroupInvalidConfiguration",
     "AutoScalingGroupNotFound",
+    "AutoScalingGroupOptInRequired",
+    "AutoScalingGroupRateLimitExceeded",
     "ClusterUnreachable",
+    "Ec2LaunchTemplateDeletionFailure",
+    "Ec2LaunchTemplateInvalidConfiguration",
+    "Ec2LaunchTemplateMaxLimitExceeded",
     "Ec2LaunchTemplateNotFound",
     "Ec2LaunchTemplateVersionMismatch",
     "Ec2SecurityGroupDeletionFailure",
     "Ec2SecurityGroupNotFound",
     "Ec2SubnetInvalidConfiguration",
+    "Ec2SubnetListTooLong",
     "Ec2SubnetMissingIpv6Assignment",
     "Ec2SubnetNotFound",
     "IamInstanceProfileNotFound",
     "IamLimitExceeded",
     "IamNodeRoleNotFound",
+    "IamThrottling",
     "InstanceLimitExceeded",
     "InsufficientFreeAddresses",
     "InternalFailure",
+    "LimitExceeded",
     "NodeCreationFailure",
+    "NodeTerminationFailure",
+    "PodEvictionFailure",
+    "SourceEc2LaunchTemplateNotFound",
+    "Unknown",
 ]
 NodegroupStatusType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATING", "DEGRADED", "DELETE_FAILED", "DELETING", "UPDATING"
 ]
 ResolveConflictsType = Literal["NONE", "OVERWRITE", "PRESERVE"]
 TaintEffectType = Literal["NO_EXECUTE", "NO_SCHEDULE", "PREFER_NO_SCHEDULE"]
 UpdateParamTypeType = Literal[
@@ -222,14 +236,15 @@
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
@@ -325,14 +340,15 @@
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
@@ -411,26 +427,28 @@
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
@@ -610,14 +628,15 @@
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

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/paginator.py` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/paginator.pyi` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/type_defs.py` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/type_defs.pyi` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/waiter.py` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks/waiter.pyi` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks.egg-info/PKG-INFO` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-eks
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EKS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EKS 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-eks)](https://pepy.tech/project/types-aiobotocore-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EKS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
+[aiobotocore.EKS 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-eks-2.5.2.post3/types_aiobotocore_eks.egg-info/SOURCES.txt` & `types-aiobotocore-eks-2.5.4/types_aiobotocore_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

