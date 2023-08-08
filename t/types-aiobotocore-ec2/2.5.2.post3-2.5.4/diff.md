# Comparing `tmp/types-aiobotocore-ec2-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-ec2-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ec2-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-ec2-2.5.4.tar", last modified: Tue Aug  8 01:23:38 2023, max compression
```

## Comparing `types-aiobotocore-ec2-2.5.2.post3.tar` & `types-aiobotocore-ec2-2.5.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.175705 types-aiobotocore-ec2-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:22:13.000000 types-aiobotocore-ec2-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    51729 2023-08-04 12:37:39.171705 types-aiobotocore-ec2-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    50227 2023-08-04 12:22:13.000000 types-aiobotocore-ec2-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:39.175705 types-aiobotocore-ec2-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:22:13.000000 types-aiobotocore-ec2-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.167704 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/
--rw-r--r--   0 runner    (1001) docker     (123)    46244 2023-08-04 12:22:13.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46242 2023-08-04 12:22:13.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:22:13.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   538805 2023-08-04 12:22:19.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   538029 2023-08-04 12:22:16.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    89586 2023-08-04 12:22:27.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    89584 2023-08-04 12:22:26.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   188566 2023-08-04 12:22:25.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)   188425 2023-08-04 12:22:23.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:22:13.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   293373 2023-08-04 12:22:22.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   292876 2023-08-04 12:22:21.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   958695 2023-08-04 12:22:52.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   957686 2023-08-04 12:22:40.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:22:13.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    40394 2023-08-04 12:22:25.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    40359 2023-08-04 12:22:25.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:39.171705 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    51729 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:38.000000 types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.830695 types-aiobotocore-ec2-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:09:45.000000 types-aiobotocore-ec2-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    51887 2023-08-08 01:23:38.830695 types-aiobotocore-ec2-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    50391 2023-08-08 01:09:45.000000 types-aiobotocore-ec2-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:38.830695 types-aiobotocore-ec2-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-08 01:09:44.000000 types-aiobotocore-ec2-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.830695 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)    46468 2023-08-08 01:09:45.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-08-08 01:09:45.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:09:45.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539019 2023-08-08 01:09:51.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   538242 2023-08-08 01:09:48.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    90331 2023-08-08 01:09:58.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90329 2023-08-08 01:09:57.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   188566 2023-08-08 01:09:55.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188425 2023-08-08 01:09:54.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:09:45.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   293404 2023-08-08 01:09:54.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292907 2023-08-08 01:09:52.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   960154 2023-08-08 01:10:20.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   959145 2023-08-08 01:10:08.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:09:45.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41581 2023-08-08 01:09:55.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41545 2023-08-08 01:09:55.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:38.830695 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    51887 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 01:23:38.000000 types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/LICENSE` & `types-aiobotocore-ec2-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-2.5.2.post3/PKG-INFO` & `types-aiobotocore-ec2-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EC2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EC2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2)](https://pepy.tech/project/types-aiobotocore-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[aiobotocore.EC2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -856,14 +856,15 @@
     NatGatewayDeletedWaiter,
     NetworkInterfaceAvailableWaiter,
     PasswordDataAvailableWaiter,
     SecurityGroupExistsWaiter,
     SnapshotCompletedWaiter,
     SnapshotImportedWaiter,
     SpotInstanceRequestFulfilledWaiter,
+    StoreImageTaskCompleteWaiter,
     SubnetAvailableWaiter,
     SystemStatusOkWaiter,
     VolumeAvailableWaiter,
     VolumeDeletedWaiter,
     VolumeInUseWaiter,
     VpcAvailableWaiter,
     VpcExistsWaiter,
@@ -925,14 +926,17 @@
         "security_group_exists"
     )
     snapshot_completed_waiter: SnapshotCompletedWaiter = client.get_waiter("snapshot_completed")
     snapshot_imported_waiter: SnapshotImportedWaiter = client.get_waiter("snapshot_imported")
     spot_instance_request_fulfilled_waiter: SpotInstanceRequestFulfilledWaiter = client.get_waiter(
         "spot_instance_request_fulfilled"
     )
+    store_image_task_complete_waiter: StoreImageTaskCompleteWaiter = client.get_waiter(
+        "store_image_task_complete"
+    )
     subnet_available_waiter: SubnetAvailableWaiter = client.get_waiter("subnet_available")
     system_status_ok_waiter: SystemStatusOkWaiter = client.get_waiter("system_status_ok")
     volume_available_waiter: VolumeAvailableWaiter = client.get_waiter("volume_available")
     volume_deleted_waiter: VolumeDeletedWaiter = client.get_waiter("volume_deleted")
     volume_in_use_waiter: VolumeInUseWaiter = client.get_waiter("volume_in_use")
     vpc_available_waiter: VpcAvailableWaiter = client.get_waiter("vpc_available")
     vpc_exists_waiter: VpcExistsWaiter = client.get_waiter("vpc_exists")
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/README.md` & `types-aiobotocore-ec2-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2)](https://pepy.tech/project/types-aiobotocore-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[aiobotocore.EC2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -824,14 +824,15 @@
     NatGatewayDeletedWaiter,
     NetworkInterfaceAvailableWaiter,
     PasswordDataAvailableWaiter,
     SecurityGroupExistsWaiter,
     SnapshotCompletedWaiter,
     SnapshotImportedWaiter,
     SpotInstanceRequestFulfilledWaiter,
+    StoreImageTaskCompleteWaiter,
     SubnetAvailableWaiter,
     SystemStatusOkWaiter,
     VolumeAvailableWaiter,
     VolumeDeletedWaiter,
     VolumeInUseWaiter,
     VpcAvailableWaiter,
     VpcExistsWaiter,
@@ -893,14 +894,17 @@
         "security_group_exists"
     )
     snapshot_completed_waiter: SnapshotCompletedWaiter = client.get_waiter("snapshot_completed")
     snapshot_imported_waiter: SnapshotImportedWaiter = client.get_waiter("snapshot_imported")
     spot_instance_request_fulfilled_waiter: SpotInstanceRequestFulfilledWaiter = client.get_waiter(
         "spot_instance_request_fulfilled"
     )
+    store_image_task_complete_waiter: StoreImageTaskCompleteWaiter = client.get_waiter(
+        "store_image_task_complete"
+    )
     subnet_available_waiter: SubnetAvailableWaiter = client.get_waiter("subnet_available")
     system_status_ok_waiter: SystemStatusOkWaiter = client.get_waiter("system_status_ok")
     volume_available_waiter: VolumeAvailableWaiter = client.get_waiter("volume_available")
     volume_deleted_waiter: VolumeDeletedWaiter = client.get_waiter("volume_deleted")
     volume_in_use_waiter: VolumeInUseWaiter = client.get_waiter("volume_in_use")
     vpc_available_waiter: VpcAvailableWaiter = client.get_waiter("vpc_available")
     vpc_exists_waiter: VpcExistsWaiter = client.get_waiter("vpc_exists")
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/setup.py` & `types-aiobotocore-ec2-2.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ec2",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_ec2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EC2 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.EC2 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/__init__.py` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,14 +168,15 @@
         SearchLocalGatewayRoutesPaginator,
         SearchTransitGatewayMulticastGroupsPaginator,
         SecurityGroupExistsWaiter,
         ServiceResource,
         SnapshotCompletedWaiter,
         SnapshotImportedWaiter,
         SpotInstanceRequestFulfilledWaiter,
+        StoreImageTaskCompleteWaiter,
         SubnetAvailableWaiter,
         SystemStatusOkWaiter,
         VolumeAvailableWaiter,
         VolumeDeletedWaiter,
         VolumeInUseWaiter,
         VpcAvailableWaiter,
         VpcExistsWaiter,
@@ -211,14 +212,15 @@
     nat_gateway_deleted_waiter: NatGatewayDeletedWaiter = client.get_waiter("nat_gateway_deleted")
     network_interface_available_waiter: NetworkInterfaceAvailableWaiter = client.get_waiter("network_interface_available")
     password_data_available_waiter: PasswordDataAvailableWaiter = client.get_waiter("password_data_available")
     security_group_exists_waiter: SecurityGroupExistsWaiter = client.get_waiter("security_group_exists")
     snapshot_completed_waiter: SnapshotCompletedWaiter = client.get_waiter("snapshot_completed")
     snapshot_imported_waiter: SnapshotImportedWaiter = client.get_waiter("snapshot_imported")
     spot_instance_request_fulfilled_waiter: SpotInstanceRequestFulfilledWaiter = client.get_waiter("spot_instance_request_fulfilled")
+    store_image_task_complete_waiter: StoreImageTaskCompleteWaiter = client.get_waiter("store_image_task_complete")
     subnet_available_waiter: SubnetAvailableWaiter = client.get_waiter("subnet_available")
     system_status_ok_waiter: SystemStatusOkWaiter = client.get_waiter("system_status_ok")
     volume_available_waiter: VolumeAvailableWaiter = client.get_waiter("volume_available")
     volume_deleted_waiter: VolumeDeletedWaiter = client.get_waiter("volume_deleted")
     volume_in_use_waiter: VolumeInUseWaiter = client.get_waiter("volume_in_use")
     vpc_available_waiter: VpcAvailableWaiter = client.get_waiter("vpc_available")
     vpc_exists_waiter: VpcExistsWaiter = client.get_waiter("vpc_exists")
@@ -530,14 +532,15 @@
     NatGatewayDeletedWaiter,
     NetworkInterfaceAvailableWaiter,
     PasswordDataAvailableWaiter,
     SecurityGroupExistsWaiter,
     SnapshotCompletedWaiter,
     SnapshotImportedWaiter,
     SpotInstanceRequestFulfilledWaiter,
+    StoreImageTaskCompleteWaiter,
     SubnetAvailableWaiter,
     SystemStatusOkWaiter,
     VolumeAvailableWaiter,
     VolumeDeletedWaiter,
     VolumeInUseWaiter,
     VpcAvailableWaiter,
     VpcExistsWaiter,
@@ -716,14 +719,15 @@
     "SearchLocalGatewayRoutesPaginator",
     "SearchTransitGatewayMulticastGroupsPaginator",
     "SecurityGroupExistsWaiter",
     "ServiceResource",
     "SnapshotCompletedWaiter",
     "SnapshotImportedWaiter",
     "SpotInstanceRequestFulfilledWaiter",
+    "StoreImageTaskCompleteWaiter",
     "SubnetAvailableWaiter",
     "SystemStatusOkWaiter",
     "VolumeAvailableWaiter",
     "VolumeDeletedWaiter",
     "VolumeInUseWaiter",
     "VpcAvailableWaiter",
     "VpcExistsWaiter",
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/__init__.pyi` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -168,14 +168,15 @@
         SearchLocalGatewayRoutesPaginator,
         SearchTransitGatewayMulticastGroupsPaginator,
         SecurityGroupExistsWaiter,
         ServiceResource,
         SnapshotCompletedWaiter,
         SnapshotImportedWaiter,
         SpotInstanceRequestFulfilledWaiter,
+        StoreImageTaskCompleteWaiter,
         SubnetAvailableWaiter,
         SystemStatusOkWaiter,
         VolumeAvailableWaiter,
         VolumeDeletedWaiter,
         VolumeInUseWaiter,
         VpcAvailableWaiter,
         VpcExistsWaiter,
@@ -211,14 +212,15 @@
     nat_gateway_deleted_waiter: NatGatewayDeletedWaiter = client.get_waiter("nat_gateway_deleted")
     network_interface_available_waiter: NetworkInterfaceAvailableWaiter = client.get_waiter("network_interface_available")
     password_data_available_waiter: PasswordDataAvailableWaiter = client.get_waiter("password_data_available")
     security_group_exists_waiter: SecurityGroupExistsWaiter = client.get_waiter("security_group_exists")
     snapshot_completed_waiter: SnapshotCompletedWaiter = client.get_waiter("snapshot_completed")
     snapshot_imported_waiter: SnapshotImportedWaiter = client.get_waiter("snapshot_imported")
     spot_instance_request_fulfilled_waiter: SpotInstanceRequestFulfilledWaiter = client.get_waiter("spot_instance_request_fulfilled")
+    store_image_task_complete_waiter: StoreImageTaskCompleteWaiter = client.get_waiter("store_image_task_complete")
     subnet_available_waiter: SubnetAvailableWaiter = client.get_waiter("subnet_available")
     system_status_ok_waiter: SystemStatusOkWaiter = client.get_waiter("system_status_ok")
     volume_available_waiter: VolumeAvailableWaiter = client.get_waiter("volume_available")
     volume_deleted_waiter: VolumeDeletedWaiter = client.get_waiter("volume_deleted")
     volume_in_use_waiter: VolumeInUseWaiter = client.get_waiter("volume_in_use")
     vpc_available_waiter: VpcAvailableWaiter = client.get_waiter("vpc_available")
     vpc_exists_waiter: VpcExistsWaiter = client.get_waiter("vpc_exists")
@@ -530,14 +532,15 @@
     NatGatewayDeletedWaiter,
     NetworkInterfaceAvailableWaiter,
     PasswordDataAvailableWaiter,
     SecurityGroupExistsWaiter,
     SnapshotCompletedWaiter,
     SnapshotImportedWaiter,
     SpotInstanceRequestFulfilledWaiter,
+    StoreImageTaskCompleteWaiter,
     SubnetAvailableWaiter,
     SystemStatusOkWaiter,
     VolumeAvailableWaiter,
     VolumeDeletedWaiter,
     VolumeInUseWaiter,
     VpcAvailableWaiter,
     VpcExistsWaiter,
@@ -714,14 +717,15 @@
     "SearchLocalGatewayRoutesPaginator",
     "SearchTransitGatewayMulticastGroupsPaginator",
     "SecurityGroupExistsWaiter",
     "ServiceResource",
     "SnapshotCompletedWaiter",
     "SnapshotImportedWaiter",
     "SpotInstanceRequestFulfilledWaiter",
+    "StoreImageTaskCompleteWaiter",
     "SubnetAvailableWaiter",
     "SystemStatusOkWaiter",
     "VolumeAvailableWaiter",
     "VolumeDeletedWaiter",
     "VolumeInUseWaiter",
     "VpcAvailableWaiter",
     "VpcExistsWaiter",
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/__main__.py` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EC2 2.5.2\nVersion:         2.5.2.post3\nBuilder version:"
+        "Type annotations for aiobotocore.EC2 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2\nOther"
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

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/client.py` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -925,14 +925,15 @@
     NatGatewayDeletedWaiter,
     NetworkInterfaceAvailableWaiter,
     PasswordDataAvailableWaiter,
     SecurityGroupExistsWaiter,
     SnapshotCompletedWaiter,
     SnapshotImportedWaiter,
     SpotInstanceRequestFulfilledWaiter,
+    StoreImageTaskCompleteWaiter,
     SubnetAvailableWaiter,
     SystemStatusOkWaiter,
     VolumeAvailableWaiter,
     VolumeDeletedWaiter,
     VolumeInUseWaiter,
     VpcAvailableWaiter,
     VpcExistsWaiter,
@@ -1515,16 +1516,16 @@
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
     ) -> AuthorizeSecurityGroupEgressResultTypeDef:
         """
-        [VPC only] Adds the specified outbound (egress) rules to a security group for
-        use with a VPC.
+        Adds the specified outbound (egress) rules to a security group for use with a
+        VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.authorize_security_group_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#authorize_security_group_egress)
         """
 
     async def authorize_security_group_ingress(
         self,
@@ -3085,15 +3086,15 @@
         IpAddressType: IpAddressTypeType = ...,
         DnsOptions: DnsOptionsSpecificationTypeDef = ...,
         ClientToken: str = ...,
         PrivateDnsEnabled: bool = ...,
         TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpcEndpointResultTypeDef:
         """
-        Creates a VPC endpoint for a specified service.
+        Creates a VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpc_endpoint)
         """
 
     async def create_vpc_endpoint_connection_notification(
         self,
@@ -4226,15 +4227,15 @@
         Filters: Sequence[FilterTypeDef] = ...,
         DryRun: bool = ...,
         InstanceIds: Sequence[str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeClassicLinkInstancesResultTypeDef:
         """
-        Describes one or more of your linked EC2-Classic instances.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_classic_link_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_classic_link_instances)
         """
 
     async def describe_client_vpn_authorization_rules(
         self,
@@ -5500,16 +5501,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_scheduled_instances)
         """
 
     async def describe_security_group_references(
         self, *, GroupId: Sequence[str], DryRun: bool = ...
     ) -> DescribeSecurityGroupReferencesResultTypeDef:
         """
-        [VPC only] Describes the VPCs on the other side of a VPC peering connection that
-        are referencing the security groups you've specified in this request.
+        Describes the VPCs on the other side of a VPC peering connection that are
+        referencing the security groups you've specified in this request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_security_group_references)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_security_group_references)
         """
 
     async def describe_security_group_rules(
         self,
@@ -5682,16 +5683,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_spot_price_history)
         """
 
     async def describe_stale_security_groups(
         self, *, VpcId: str, DryRun: bool = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeStaleSecurityGroupsResultTypeDef:
         """
-        [VPC only] Describes the stale security group rules for security groups in a
-        specified VPC.
+        Describes the stale security group rules for security groups in a specified VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_stale_security_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_stale_security_groups)
         """
 
     async def describe_store_image_tasks(
         self,
@@ -6120,15 +6120,15 @@
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         DryRun: bool = ...,
         VpcIds: Sequence[str] = ...
     ) -> DescribeVpcClassicLinkResultTypeDef:
         """
-        Describes the ClassicLink status of one or more VPCs.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_vpc_classic_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_vpc_classic_link)
         """
 
     async def describe_vpc_classic_link_dns_support(
         self, *, MaxResults: int = ..., NextToken: str = ..., VpcIds: Sequence[str] = ...
@@ -6491,25 +6491,25 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#disable_vgw_route_propagation)
         """
 
     async def disable_vpc_classic_link(
         self, *, VpcId: str, DryRun: bool = ...
     ) -> DisableVpcClassicLinkResultTypeDef:
         """
-        Disables ClassicLink for a VPC.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.disable_vpc_classic_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#disable_vpc_classic_link)
         """
 
     async def disable_vpc_classic_link_dns_support(
         self, *, VpcId: str = ...
     ) -> DisableVpcClassicLinkDnsSupportResultTypeDef:
         """
-        Disables ClassicLink DNS support for a VPC.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.disable_vpc_classic_link_dns_support)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#disable_vpc_classic_link_dns_support)
         """
 
     async def disassociate_address(
         self, *, AssociationId: str = ..., PublicIp: str = ..., DryRun: bool = ...
@@ -7566,15 +7566,15 @@
         Platform: Literal["Windows"],
         Description: str = ...,
         DiskImages: Sequence[DiskImageTypeDef] = ...,
         DryRun: bool = ...,
         LaunchSpecification: ImportInstanceLaunchSpecificationTypeDef = ...
     ) -> ImportInstanceResultTypeDef:
         """
-        Creates an import instance task using metadata from the specified disk image.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#import_instance)
         """
 
     async def import_key_pair(
         self,
@@ -8629,15 +8629,16 @@
         *,
         VpcPeeringConnectionId: str,
         AccepterPeeringConnectionOptions: PeeringConnectionOptionsRequestTypeDef = ...,
         DryRun: bool = ...,
         RequesterPeeringConnectionOptions: PeeringConnectionOptionsRequestTypeDef = ...
     ) -> ModifyVpcPeeringConnectionOptionsResultTypeDef:
         """
-        .
+        Modifies the VPC peering connection options on one side of a VPC peering
+        connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.modify_vpc_peering_connection_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#modify_vpc_peering_connection_options)
         """
 
     async def modify_vpc_tenancy(
         self, *, VpcId: str, InstanceTenancy: Literal["default"], DryRun: bool = ...
@@ -9327,16 +9328,15 @@
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
     ) -> RevokeSecurityGroupEgressResultTypeDef:
         """
-        [VPC only] Removes the specified outbound (egress) rules from a security group
-        for EC2-VPC.
+        Removes the specified outbound (egress) rules from the specified security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.revoke_security_group_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#revoke_security_group_egress)
         """
 
     async def revoke_security_group_ingress(
         self,
@@ -9642,15 +9642,15 @@
         DryRun: bool = ...,
         GroupId: str = ...,
         GroupName: str = ...,
         IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         SecurityGroupRuleDescriptions: Sequence[SecurityGroupRuleDescriptionTypeDef] = ...
     ) -> UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef:
         """
-        [VPC only] Updates the description of an egress (outbound) security group rule.
+        Updates the description of an egress (outbound) security group rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.update_security_group_rule_descriptions_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#update_security_group_rule_descriptions_egress)
         """
 
     async def update_security_group_rule_descriptions_ingress(
         self,
@@ -11100,14 +11100,23 @@
     ) -> SpotInstanceRequestFulfilledWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#get_waiter)
         """
 
     @overload
+    def get_waiter(
+        self, waiter_name: Literal["store_image_task_complete"]
+    ) -> StoreImageTaskCompleteWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.get_waiter)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#get_waiter)
+        """
+
+    @overload
     def get_waiter(self, waiter_name: Literal["subnet_available"]) -> SubnetAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#get_waiter)
         """
 
     @overload
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/client.pyi` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -925,14 +925,15 @@
     NatGatewayDeletedWaiter,
     NetworkInterfaceAvailableWaiter,
     PasswordDataAvailableWaiter,
     SecurityGroupExistsWaiter,
     SnapshotCompletedWaiter,
     SnapshotImportedWaiter,
     SpotInstanceRequestFulfilledWaiter,
+    StoreImageTaskCompleteWaiter,
     SubnetAvailableWaiter,
     SystemStatusOkWaiter,
     VolumeAvailableWaiter,
     VolumeDeletedWaiter,
     VolumeInUseWaiter,
     VpcAvailableWaiter,
     VpcExistsWaiter,
@@ -1473,16 +1474,16 @@
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
     ) -> AuthorizeSecurityGroupEgressResultTypeDef:
         """
-        [VPC only] Adds the specified outbound (egress) rules to a security group for
-        use with a VPC.
+        Adds the specified outbound (egress) rules to a security group for use with a
+        VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.authorize_security_group_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#authorize_security_group_egress)
         """
     async def authorize_security_group_ingress(
         self,
         *,
@@ -2949,15 +2950,15 @@
         IpAddressType: IpAddressTypeType = ...,
         DnsOptions: DnsOptionsSpecificationTypeDef = ...,
         ClientToken: str = ...,
         PrivateDnsEnabled: bool = ...,
         TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpcEndpointResultTypeDef:
         """
-        Creates a VPC endpoint for a specified service.
+        Creates a VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpc_endpoint)
         """
     async def create_vpc_endpoint_connection_notification(
         self,
         *,
@@ -3990,15 +3991,15 @@
         Filters: Sequence[FilterTypeDef] = ...,
         DryRun: bool = ...,
         InstanceIds: Sequence[str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeClassicLinkInstancesResultTypeDef:
         """
-        Describes one or more of your linked EC2-Classic instances.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_classic_link_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_classic_link_instances)
         """
     async def describe_client_vpn_authorization_rules(
         self,
         *,
@@ -5183,16 +5184,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_scheduled_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_scheduled_instances)
         """
     async def describe_security_group_references(
         self, *, GroupId: Sequence[str], DryRun: bool = ...
     ) -> DescribeSecurityGroupReferencesResultTypeDef:
         """
-        [VPC only] Describes the VPCs on the other side of a VPC peering connection that
-        are referencing the security groups you've specified in this request.
+        Describes the VPCs on the other side of a VPC peering connection that are
+        referencing the security groups you've specified in this request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_security_group_references)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_security_group_references)
         """
     async def describe_security_group_rules(
         self,
         *,
@@ -5353,16 +5354,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_spot_price_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_spot_price_history)
         """
     async def describe_stale_security_groups(
         self, *, VpcId: str, DryRun: bool = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeStaleSecurityGroupsResultTypeDef:
         """
-        [VPC only] Describes the stale security group rules for security groups in a
-        specified VPC.
+        Describes the stale security group rules for security groups in a specified VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_stale_security_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_stale_security_groups)
         """
     async def describe_store_image_tasks(
         self,
         *,
@@ -5763,15 +5763,15 @@
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         DryRun: bool = ...,
         VpcIds: Sequence[str] = ...
     ) -> DescribeVpcClassicLinkResultTypeDef:
         """
-        Describes the ClassicLink status of one or more VPCs.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_vpc_classic_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#describe_vpc_classic_link)
         """
     async def describe_vpc_classic_link_dns_support(
         self, *, MaxResults: int = ..., NextToken: str = ..., VpcIds: Sequence[str] = ...
     ) -> DescribeVpcClassicLinkDnsSupportResultTypeDef:
@@ -6106,24 +6106,24 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.disable_vgw_route_propagation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#disable_vgw_route_propagation)
         """
     async def disable_vpc_classic_link(
         self, *, VpcId: str, DryRun: bool = ...
     ) -> DisableVpcClassicLinkResultTypeDef:
         """
-        Disables ClassicLink for a VPC.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.disable_vpc_classic_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#disable_vpc_classic_link)
         """
     async def disable_vpc_classic_link_dns_support(
         self, *, VpcId: str = ...
     ) -> DisableVpcClassicLinkDnsSupportResultTypeDef:
         """
-        Disables ClassicLink DNS support for a VPC.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.disable_vpc_classic_link_dns_support)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#disable_vpc_classic_link_dns_support)
         """
     async def disassociate_address(
         self, *, AssociationId: str = ..., PublicIp: str = ..., DryRun: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
@@ -7101,15 +7101,15 @@
         Platform: Literal["Windows"],
         Description: str = ...,
         DiskImages: Sequence[DiskImageTypeDef] = ...,
         DryRun: bool = ...,
         LaunchSpecification: ImportInstanceLaunchSpecificationTypeDef = ...
     ) -> ImportInstanceResultTypeDef:
         """
-        Creates an import instance task using metadata from the specified disk image.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#import_instance)
         """
     async def import_key_pair(
         self,
         *,
@@ -8100,15 +8100,16 @@
         *,
         VpcPeeringConnectionId: str,
         AccepterPeeringConnectionOptions: PeeringConnectionOptionsRequestTypeDef = ...,
         DryRun: bool = ...,
         RequesterPeeringConnectionOptions: PeeringConnectionOptionsRequestTypeDef = ...
     ) -> ModifyVpcPeeringConnectionOptionsResultTypeDef:
         """
-        .
+        Modifies the VPC peering connection options on one side of a VPC peering
+        connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.modify_vpc_peering_connection_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#modify_vpc_peering_connection_options)
         """
     async def modify_vpc_tenancy(
         self, *, VpcId: str, InstanceTenancy: Literal["default"], DryRun: bool = ...
     ) -> ModifyVpcTenancyResultTypeDef:
@@ -8747,16 +8748,15 @@
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
     ) -> RevokeSecurityGroupEgressResultTypeDef:
         """
-        [VPC only] Removes the specified outbound (egress) rules from a security group
-        for EC2-VPC.
+        Removes the specified outbound (egress) rules from the specified security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.revoke_security_group_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#revoke_security_group_egress)
         """
     async def revoke_security_group_ingress(
         self,
         *,
@@ -9043,15 +9043,15 @@
         DryRun: bool = ...,
         GroupId: str = ...,
         GroupName: str = ...,
         IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         SecurityGroupRuleDescriptions: Sequence[SecurityGroupRuleDescriptionTypeDef] = ...
     ) -> UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef:
         """
-        [VPC only] Updates the description of an egress (outbound) security group rule.
+        Updates the description of an egress (outbound) security group rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.update_security_group_rule_descriptions_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#update_security_group_rule_descriptions_egress)
         """
     async def update_security_group_rule_descriptions_ingress(
         self,
         *,
@@ -10336,14 +10336,22 @@
         self, waiter_name: Literal["spot_instance_request_fulfilled"]
     ) -> SpotInstanceRequestFulfilledWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#get_waiter)
         """
     @overload
+    def get_waiter(
+        self, waiter_name: Literal["store_image_task_complete"]
+    ) -> StoreImageTaskCompleteWaiter:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.get_waiter)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#get_waiter)
+        """
+    @overload
     def get_waiter(self, waiter_name: Literal["subnet_available"]) -> SubnetAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#get_waiter)
         """
     @overload
     def get_waiter(self, waiter_name: Literal["system_status_ok"]) -> SystemStatusOkWaiter:
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/literals.py` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,16 @@
     "NatGatewayStateType",
     "NetworkInterfaceAttributeType",
     "NetworkInterfaceAvailableWaiterName",
     "NetworkInterfaceCreationTypeType",
     "NetworkInterfacePermissionStateCodeType",
     "NetworkInterfaceStatusType",
     "NetworkInterfaceTypeType",
+    "NitroEnclavesSupportType",
+    "NitroTpmSupportType",
     "OfferingClassTypeType",
     "OfferingTypeValuesType",
     "OnDemandAllocationStrategyType",
     "OperationTypeType",
     "PartitionLoadFrequencyType",
     "PasswordDataAvailableWaiterName",
     "PayerResponsibilityType",
@@ -396,14 +398,15 @@
     "ResetImageAttributeNameType",
     "ResourceTypeType",
     "RootDeviceTypeType",
     "RouteOriginType",
     "RouteStateType",
     "RouteTableAssociationStateCodeType",
     "RuleActionType",
+    "SSETypeType",
     "SearchLocalGatewayRoutesPaginatorName",
     "SearchTransitGatewayMulticastGroupsPaginatorName",
     "SecurityGroupExistsWaiterName",
     "SelfServicePortalType",
     "ServiceConnectivityTypeType",
     "ServiceStateType",
     "ServiceTypeType",
@@ -421,14 +424,15 @@
     "StateType",
     "StaticSourcesSupportValueType",
     "StatisticTypeType",
     "StatusNameType",
     "StatusType",
     "StatusTypeType",
     "StorageTierType",
+    "StoreImageTaskCompleteWaiterName",
     "SubnetAvailableWaiterName",
     "SubnetCidrBlockStateCodeType",
     "SubnetCidrReservationTypeType",
     "SubnetStateType",
     "SummaryStatusType",
     "SupportedAdditionalProcessorFeatureType",
     "SystemStatusOkWaiterName",
@@ -1125,14 +1129,22 @@
     "c7g.2xlarge",
     "c7g.4xlarge",
     "c7g.8xlarge",
     "c7g.large",
     "c7g.medium",
     "c7g.metal",
     "c7g.xlarge",
+    "c7gn.12xlarge",
+    "c7gn.16xlarge",
+    "c7gn.2xlarge",
+    "c7gn.4xlarge",
+    "c7gn.8xlarge",
+    "c7gn.large",
+    "c7gn.medium",
+    "c7gn.xlarge",
     "cc1.4xlarge",
     "cc2.8xlarge",
     "cg1.4xlarge",
     "cr1.8xlarge",
     "d2.2xlarge",
     "d2.4xlarge",
     "d2.8xlarge",
@@ -1186,14 +1198,17 @@
     "h1.16xlarge",
     "h1.2xlarge",
     "h1.4xlarge",
     "h1.8xlarge",
     "hi1.4xlarge",
     "hpc6a.48xlarge",
     "hpc6id.32xlarge",
+    "hpc7g.16xlarge",
+    "hpc7g.4xlarge",
+    "hpc7g.8xlarge",
     "hs1.8xlarge",
     "i2.2xlarge",
     "i2.4xlarge",
     "i2.8xlarge",
     "i2.xlarge",
     "i3.16xlarge",
     "i3.2xlarge",
@@ -1808,14 +1823,16 @@
     "natGateway",
     "network_load_balancer",
     "quicksight",
     "transit_gateway",
     "trunk",
     "vpc_endpoint",
 ]
+NitroEnclavesSupportType = Literal["supported", "unsupported"]
+NitroTpmSupportType = Literal["supported", "unsupported"]
 OfferingClassTypeType = Literal["convertible", "standard"]
 OfferingTypeValuesType = Literal[
     "All Upfront",
     "Heavy Utilization",
     "Light Utilization",
     "Medium Utilization",
     "No Upfront",
@@ -1970,14 +1987,15 @@
 RootDeviceTypeType = Literal["ebs", "instance-store"]
 RouteOriginType = Literal["CreateRoute", "CreateRouteTable", "EnableVgwRoutePropagation"]
 RouteStateType = Literal["active", "blackhole"]
 RouteTableAssociationStateCodeType = Literal[
     "associated", "associating", "disassociated", "disassociating", "failed"
 ]
 RuleActionType = Literal["allow", "deny"]
+SSETypeType = Literal["none", "sse-ebs", "sse-kms"]
 SearchLocalGatewayRoutesPaginatorName = Literal["search_local_gateway_routes"]
 SearchTransitGatewayMulticastGroupsPaginatorName = Literal[
     "search_transit_gateway_multicast_groups"
 ]
 SecurityGroupExistsWaiterName = Literal["security_group_exists"]
 SelfServicePortalType = Literal["disabled", "enabled"]
 ServiceConnectivityTypeType = Literal["ipv4", "ipv6"]
@@ -1993,15 +2011,15 @@
     "capacity-optimized-prioritized",
     "diversified",
     "lowest-price",
     "price-capacity-optimized",
 ]
 SpotInstanceInterruptionBehaviorType = Literal["hibernate", "stop", "terminate"]
 SpotInstanceRequestFulfilledWaiterName = Literal["spot_instance_request_fulfilled"]
-SpotInstanceStateType = Literal["active", "cancelled", "closed", "failed", "open"]
+SpotInstanceStateType = Literal["active", "cancelled", "closed", "disabled", "failed", "open"]
 SpotInstanceTypeType = Literal["one-time", "persistent"]
 SpreadLevelType = Literal["host", "rack"]
 StateType = Literal[
     "Available",
     "Deleted",
     "Deleting",
     "Expired",
@@ -2012,14 +2030,15 @@
 ]
 StaticSourcesSupportValueType = Literal["disable", "enable"]
 StatisticTypeType = Literal["p50"]
 StatusNameType = Literal["reachability"]
 StatusType = Literal["InClassic", "InVpc", "MoveInProgress"]
 StatusTypeType = Literal["failed", "initializing", "insufficient-data", "passed"]
 StorageTierType = Literal["archive", "standard"]
+StoreImageTaskCompleteWaiterName = Literal["store_image_task_complete"]
 SubnetAvailableWaiterName = Literal["subnet_available"]
 SubnetCidrBlockStateCodeType = Literal[
     "associated", "associating", "disassociated", "disassociating", "failed", "failing"
 ]
 SubnetCidrReservationTypeType = Literal["explicit", "prefix"]
 SubnetStateType = Literal["available", "pending"]
 SummaryStatusType = Literal["impaired", "initializing", "insufficient-data", "not-applicable", "ok"]
@@ -2171,14 +2190,15 @@
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
@@ -2274,14 +2294,15 @@
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
@@ -2360,26 +2381,28 @@
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
@@ -2684,14 +2707,15 @@
     "nat_gateway_deleted",
     "network_interface_available",
     "password_data_available",
     "security_group_exists",
     "snapshot_completed",
     "snapshot_imported",
     "spot_instance_request_fulfilled",
+    "store_image_task_complete",
     "subnet_available",
     "system_status_ok",
     "volume_available",
     "volume_deleted",
     "volume_in_use",
     "vpc_available",
     "vpc_exists",
@@ -2717,14 +2741,15 @@
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

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/literals.pyi` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -360,14 +360,16 @@
     "NatGatewayStateType",
     "NetworkInterfaceAttributeType",
     "NetworkInterfaceAvailableWaiterName",
     "NetworkInterfaceCreationTypeType",
     "NetworkInterfacePermissionStateCodeType",
     "NetworkInterfaceStatusType",
     "NetworkInterfaceTypeType",
+    "NitroEnclavesSupportType",
+    "NitroTpmSupportType",
     "OfferingClassTypeType",
     "OfferingTypeValuesType",
     "OnDemandAllocationStrategyType",
     "OperationTypeType",
     "PartitionLoadFrequencyType",
     "PasswordDataAvailableWaiterName",
     "PayerResponsibilityType",
@@ -395,14 +397,15 @@
     "ResetImageAttributeNameType",
     "ResourceTypeType",
     "RootDeviceTypeType",
     "RouteOriginType",
     "RouteStateType",
     "RouteTableAssociationStateCodeType",
     "RuleActionType",
+    "SSETypeType",
     "SearchLocalGatewayRoutesPaginatorName",
     "SearchTransitGatewayMulticastGroupsPaginatorName",
     "SecurityGroupExistsWaiterName",
     "SelfServicePortalType",
     "ServiceConnectivityTypeType",
     "ServiceStateType",
     "ServiceTypeType",
@@ -420,14 +423,15 @@
     "StateType",
     "StaticSourcesSupportValueType",
     "StatisticTypeType",
     "StatusNameType",
     "StatusType",
     "StatusTypeType",
     "StorageTierType",
+    "StoreImageTaskCompleteWaiterName",
     "SubnetAvailableWaiterName",
     "SubnetCidrBlockStateCodeType",
     "SubnetCidrReservationTypeType",
     "SubnetStateType",
     "SummaryStatusType",
     "SupportedAdditionalProcessorFeatureType",
     "SystemStatusOkWaiterName",
@@ -1123,14 +1127,22 @@
     "c7g.2xlarge",
     "c7g.4xlarge",
     "c7g.8xlarge",
     "c7g.large",
     "c7g.medium",
     "c7g.metal",
     "c7g.xlarge",
+    "c7gn.12xlarge",
+    "c7gn.16xlarge",
+    "c7gn.2xlarge",
+    "c7gn.4xlarge",
+    "c7gn.8xlarge",
+    "c7gn.large",
+    "c7gn.medium",
+    "c7gn.xlarge",
     "cc1.4xlarge",
     "cc2.8xlarge",
     "cg1.4xlarge",
     "cr1.8xlarge",
     "d2.2xlarge",
     "d2.4xlarge",
     "d2.8xlarge",
@@ -1184,14 +1196,17 @@
     "h1.16xlarge",
     "h1.2xlarge",
     "h1.4xlarge",
     "h1.8xlarge",
     "hi1.4xlarge",
     "hpc6a.48xlarge",
     "hpc6id.32xlarge",
+    "hpc7g.16xlarge",
+    "hpc7g.4xlarge",
+    "hpc7g.8xlarge",
     "hs1.8xlarge",
     "i2.2xlarge",
     "i2.4xlarge",
     "i2.8xlarge",
     "i2.xlarge",
     "i3.16xlarge",
     "i3.2xlarge",
@@ -1806,14 +1821,16 @@
     "natGateway",
     "network_load_balancer",
     "quicksight",
     "transit_gateway",
     "trunk",
     "vpc_endpoint",
 ]
+NitroEnclavesSupportType = Literal["supported", "unsupported"]
+NitroTpmSupportType = Literal["supported", "unsupported"]
 OfferingClassTypeType = Literal["convertible", "standard"]
 OfferingTypeValuesType = Literal[
     "All Upfront",
     "Heavy Utilization",
     "Light Utilization",
     "Medium Utilization",
     "No Upfront",
@@ -1968,14 +1985,15 @@
 RootDeviceTypeType = Literal["ebs", "instance-store"]
 RouteOriginType = Literal["CreateRoute", "CreateRouteTable", "EnableVgwRoutePropagation"]
 RouteStateType = Literal["active", "blackhole"]
 RouteTableAssociationStateCodeType = Literal[
     "associated", "associating", "disassociated", "disassociating", "failed"
 ]
 RuleActionType = Literal["allow", "deny"]
+SSETypeType = Literal["none", "sse-ebs", "sse-kms"]
 SearchLocalGatewayRoutesPaginatorName = Literal["search_local_gateway_routes"]
 SearchTransitGatewayMulticastGroupsPaginatorName = Literal[
     "search_transit_gateway_multicast_groups"
 ]
 SecurityGroupExistsWaiterName = Literal["security_group_exists"]
 SelfServicePortalType = Literal["disabled", "enabled"]
 ServiceConnectivityTypeType = Literal["ipv4", "ipv6"]
@@ -1991,15 +2009,15 @@
     "capacity-optimized-prioritized",
     "diversified",
     "lowest-price",
     "price-capacity-optimized",
 ]
 SpotInstanceInterruptionBehaviorType = Literal["hibernate", "stop", "terminate"]
 SpotInstanceRequestFulfilledWaiterName = Literal["spot_instance_request_fulfilled"]
-SpotInstanceStateType = Literal["active", "cancelled", "closed", "failed", "open"]
+SpotInstanceStateType = Literal["active", "cancelled", "closed", "disabled", "failed", "open"]
 SpotInstanceTypeType = Literal["one-time", "persistent"]
 SpreadLevelType = Literal["host", "rack"]
 StateType = Literal[
     "Available",
     "Deleted",
     "Deleting",
     "Expired",
@@ -2010,14 +2028,15 @@
 ]
 StaticSourcesSupportValueType = Literal["disable", "enable"]
 StatisticTypeType = Literal["p50"]
 StatusNameType = Literal["reachability"]
 StatusType = Literal["InClassic", "InVpc", "MoveInProgress"]
 StatusTypeType = Literal["failed", "initializing", "insufficient-data", "passed"]
 StorageTierType = Literal["archive", "standard"]
+StoreImageTaskCompleteWaiterName = Literal["store_image_task_complete"]
 SubnetAvailableWaiterName = Literal["subnet_available"]
 SubnetCidrBlockStateCodeType = Literal[
     "associated", "associating", "disassociated", "disassociating", "failed", "failing"
 ]
 SubnetCidrReservationTypeType = Literal["explicit", "prefix"]
 SubnetStateType = Literal["available", "pending"]
 SummaryStatusType = Literal["impaired", "initializing", "insufficient-data", "not-applicable", "ok"]
@@ -2169,14 +2188,15 @@
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
@@ -2272,14 +2292,15 @@
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
@@ -2358,26 +2379,28 @@
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
@@ -2682,14 +2705,15 @@
     "nat_gateway_deleted",
     "network_interface_available",
     "password_data_available",
     "security_group_exists",
     "snapshot_completed",
     "snapshot_imported",
     "spot_instance_request_fulfilled",
+    "store_image_task_complete",
     "subnet_available",
     "system_status_ok",
     "volume_available",
     "volume_deleted",
     "volume_in_use",
     "vpc_available",
     "vpc_exists",
@@ -2715,14 +2739,15 @@
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

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/paginator.py` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/paginator.pyi` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/service_resource.py` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     RouteOriginType,
     RouteStateType,
     RuleActionType,
     ShutdownBehaviorType,
     SnapshotAttributeNameType,
     SnapshotStateType,
     SpreadLevelType,
+    SSETypeType,
     StorageTierType,
     SubnetStateType,
     TenancyType,
     VirtualizationTypeType,
     VolumeAttributeNameType,
     VolumeStateType,
     VolumeTypeType,
@@ -3381,16 +3382,16 @@
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
     ) -> AuthorizeSecurityGroupEgressResultTypeDef:
         """
-        [VPC only] Adds the specified outbound (egress) rules to a security group for
-        use with a VPC.
+        Adds the specified outbound (egress) rules to a security group for use with a
+        VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.SecurityGroup.authorize_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#securitygroupauthorize_egress-method)
         """
 
     async def authorize_ingress(
         self,
@@ -3496,16 +3497,15 @@
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
     ) -> RevokeSecurityGroupEgressResultTypeDef:
         """
-        [VPC only] Removes the specified outbound (egress) rules from a security group
-        for EC2-VPC.
+        Removes the specified outbound (egress) rules from the specified security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.SecurityGroup.revoke_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#securitygrouprevoke_egress-method)
         """
 
     async def revoke_ingress(
         self,
@@ -3551,14 +3551,15 @@
     volume_id: Awaitable[str]
     volume_size: Awaitable[int]
     owner_alias: Awaitable[str]
     outpost_arn: Awaitable[str]
     tags: Awaitable[List[TagTypeDef]]
     storage_tier: Awaitable[StorageTierType]
     restore_expiry_time: Awaitable[datetime]
+    sse_type: Awaitable[SSETypeType]
     id: str
     volume: "Volume"
 
     async def copy(
         self,
         *,
         SourceRegion: str,
@@ -4441,14 +4442,15 @@
     volume_id: Awaitable[str]
     iops: Awaitable[int]
     tags: Awaitable[List[TagTypeDef]]
     volume_type: Awaitable[VolumeTypeType]
     fast_restored: Awaitable[bool]
     multi_attach_enabled: Awaitable[bool]
     throughput: Awaitable[int]
+    sse_type: Awaitable[SSETypeType]
     id: str
     snapshots: VolumeSnapshotsCollection
 
     async def attach_to_instance(
         self, *, Device: str, InstanceId: str, DryRun: bool = ...
     ) -> VolumeAttachmentResponseTypeDef:
         """
@@ -5109,15 +5111,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#vpcdetach_internet_gateway-method)
         """
 
     async def disable_classic_link(
         self, *, DryRun: bool = ...
     ) -> DisableVpcClassicLinkResultTypeDef:
         """
-        Disables ClassicLink for a VPC.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Vpc.disable_classic_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#vpcdisable_classic_link-method)
         """
 
     async def enable_classic_link(self, *, DryRun: bool = ...) -> EnableVpcClassicLinkResultTypeDef:
         """
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/service_resource.pyi` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     RouteOriginType,
     RouteStateType,
     RuleActionType,
     ShutdownBehaviorType,
     SnapshotAttributeNameType,
     SnapshotStateType,
     SpreadLevelType,
+    SSETypeType,
     StorageTierType,
     SubnetStateType,
     TenancyType,
     VirtualizationTypeType,
     VolumeAttributeNameType,
     VolumeStateType,
     VolumeTypeType,
@@ -3054,16 +3055,16 @@
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
     ) -> AuthorizeSecurityGroupEgressResultTypeDef:
         """
-        [VPC only] Adds the specified outbound (egress) rules to a security group for
-        use with a VPC.
+        Adds the specified outbound (egress) rules to a security group for use with a
+        VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.SecurityGroup.authorize_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#securitygroupauthorize_egress-method)
         """
     async def authorize_ingress(
         self,
         *,
@@ -3162,16 +3163,15 @@
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
     ) -> RevokeSecurityGroupEgressResultTypeDef:
         """
-        [VPC only] Removes the specified outbound (egress) rules from a security group
-        for EC2-VPC.
+        Removes the specified outbound (egress) rules from the specified security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.SecurityGroup.revoke_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#securitygrouprevoke_egress-method)
         """
     async def revoke_ingress(
         self,
         *,
@@ -3214,14 +3214,15 @@
     volume_id: Awaitable[str]
     volume_size: Awaitable[int]
     owner_alias: Awaitable[str]
     outpost_arn: Awaitable[str]
     tags: Awaitable[List[TagTypeDef]]
     storage_tier: Awaitable[StorageTierType]
     restore_expiry_time: Awaitable[datetime]
+    sse_type: Awaitable[SSETypeType]
     id: str
     volume: "Volume"
 
     async def copy(
         self,
         *,
         SourceRegion: str,
@@ -4035,14 +4036,15 @@
     volume_id: Awaitable[str]
     iops: Awaitable[int]
     tags: Awaitable[List[TagTypeDef]]
     volume_type: Awaitable[VolumeTypeType]
     fast_restored: Awaitable[bool]
     multi_attach_enabled: Awaitable[bool]
     throughput: Awaitable[int]
+    sse_type: Awaitable[SSETypeType]
     id: str
     snapshots: VolumeSnapshotsCollection
 
     async def attach_to_instance(
         self, *, Device: str, InstanceId: str, DryRun: bool = ...
     ) -> VolumeAttachmentResponseTypeDef:
         """
@@ -4662,15 +4664,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Vpc.detach_internet_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#vpcdetach_internet_gateway-method)
         """
     async def disable_classic_link(
         self, *, DryRun: bool = ...
     ) -> DisableVpcClassicLinkResultTypeDef:
         """
-        Disables ClassicLink for a VPC.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Vpc.disable_classic_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#vpcdisable_classic_link-method)
         """
     async def enable_classic_link(self, *, DryRun: bool = ...) -> EnableVpcClassicLinkResultTypeDef:
         """
         .
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/type_defs.py` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,16 @@
     NatGatewayAddressStatusType,
     NatGatewayStateType,
     NetworkInterfaceAttributeType,
     NetworkInterfaceCreationTypeType,
     NetworkInterfacePermissionStateCodeType,
     NetworkInterfaceStatusType,
     NetworkInterfaceTypeType,
+    NitroEnclavesSupportType,
+    NitroTpmSupportType,
     OfferingClassTypeType,
     OfferingTypeValuesType,
     OnDemandAllocationStrategyType,
     OperationTypeType,
     PartitionLoadFrequencyType,
     PaymentOptionType,
     PeriodTypeType,
@@ -226,14 +228,15 @@
     SnapshotAttributeNameType,
     SnapshotStateType,
     SpotAllocationStrategyType,
     SpotInstanceInterruptionBehaviorType,
     SpotInstanceStateType,
     SpotInstanceTypeType,
     SpreadLevelType,
+    SSETypeType,
     StateType,
     StaticSourcesSupportValueType,
     StatusType,
     StatusTypeType,
     StorageTierType,
     SubnetCidrBlockStateCodeType,
     SubnetCidrReservationTypeType,
@@ -810,15 +813,15 @@
     "LaunchPermissionTypeDef",
     "UserBucketTypeDef",
     "ImageRecycleBinInfoTypeDef",
     "ImportClientVpnClientCertificateRevocationListRequestRequestTypeDef",
     "ImportImageLicenseConfigurationRequestTypeDef",
     "ImportImageLicenseConfigurationResponseTypeDef",
     "UserDataTypeDef",
-    "InferenceDeviceInfoTypeDef",
+    "InferenceDeviceMemoryInfoTypeDef",
     "InstanceCountTypeDef",
     "InstanceCreditSpecificationRequestTypeDef",
     "InstanceEventWindowTimeRangeTypeDef",
     "InstanceIpv4PrefixTypeDef",
     "InstanceIpv6AddressRequestTypeDef",
     "InstanceIpv6PrefixTypeDef",
     "InstanceMaintenanceOptionsRequestTypeDef",
@@ -842,14 +845,15 @@
     "VCpuCountRangeTypeDef",
     "InstanceStateTypeDef",
     "InstanceStatusDetailsTypeDef",
     "InstanceStatusEventTypeDef",
     "LicenseConfigurationTypeDef",
     "PrivateDnsNameOptionsResponseTypeDef",
     "MemoryInfoTypeDef",
+    "NitroTpmInfoTypeDef",
     "PlacementGroupInfoTypeDef",
     "ProcessorInfoTypeDef",
     "VCpuInfoTypeDef",
     "IpRangeTypeDef",
     "Ipv6RangeTypeDef",
     "PrefixListIdTypeDef",
     "UserIdGroupPairTypeDef",
@@ -1087,15 +1091,14 @@
     "VerifiedAccessEndpointStatusTypeDef",
     "VerifiedAccessTrustProviderCondensedTypeDef",
     "VerifiedAccessLogCloudWatchLogsDestinationOptionsTypeDef",
     "VerifiedAccessLogDeliveryStatusTypeDef",
     "VerifiedAccessLogKinesisDataFirehoseDestinationOptionsTypeDef",
     "VerifiedAccessLogS3DestinationOptionsTypeDef",
     "VgwTelemetryTypeDef",
-    "VolumeAttachmentTypeDef",
     "VolumeStatusActionTypeDef",
     "VolumeStatusAttachmentStatusTypeDef",
     "VolumeStatusDetailsTypeDef",
     "VolumeStatusEventTypeDef",
     "VpcCidrBlockStateTypeDef",
     "VpcPeeringConnectionOptionsDescriptionTypeDef",
     "VpcPeeringConnectionStateReasonTypeDef",
@@ -1226,14 +1229,15 @@
     "StartVpcEndpointServicePrivateDnsVerificationResultTypeDef",
     "StateReasonResponseTypeDef",
     "StateReasonTypeDef",
     "UnassignIpv6AddressesResultTypeDef",
     "UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef",
     "UpdateSecurityGroupRuleDescriptionsIngressResultTypeDef",
     "VolumeAttachmentResponseTypeDef",
+    "VolumeAttachmentTypeDef",
     "VpcPeeringConnectionStateReasonResponseTypeDef",
     "AcceptReservedInstancesExchangeQuoteRequestRequestTypeDef",
     "GetReservedInstancesExchangeQuoteRequestRequestTypeDef",
     "AccountAttributeTypeDef",
     "DescribeFleetInstancesResultTypeDef",
     "DescribeSpotFleetInstancesResponseTypeDef",
     "ModifyVpcEndpointServicePermissionsResultTypeDef",
@@ -1720,14 +1724,15 @@
     "DescribeKeyPairsRequestKeyPairExistsWaitTypeDef",
     "DescribeNatGatewaysRequestNatGatewayAvailableWaitTypeDef",
     "DescribeNatGatewaysRequestNatGatewayDeletedWaitTypeDef",
     "DescribeNetworkInterfacesRequestNetworkInterfaceAvailableWaitTypeDef",
     "DescribeSecurityGroupsRequestSecurityGroupExistsWaitTypeDef",
     "DescribeSnapshotsRequestSnapshotCompletedWaitTypeDef",
     "DescribeSpotInstanceRequestsRequestSpotInstanceRequestFulfilledWaitTypeDef",
+    "DescribeStoreImageTasksRequestStoreImageTaskCompleteWaitTypeDef",
     "DescribeSubnetsRequestSubnetAvailableWaitTypeDef",
     "DescribeVolumesRequestVolumeAvailableWaitTypeDef",
     "DescribeVolumesRequestVolumeDeletedWaitTypeDef",
     "DescribeVolumesRequestVolumeInUseWaitTypeDef",
     "DescribeVpcPeeringConnectionsRequestVpcPeeringConnectionDeletedWaitTypeDef",
     "DescribeVpcPeeringConnectionsRequestVpcPeeringConnectionExistsWaitTypeDef",
     "DescribeVpcsRequestVpcAvailableWaitTypeDef",
@@ -1804,15 +1809,15 @@
     "GpuDeviceInfoTypeDef",
     "IamInstanceProfileAssociationTypeDef",
     "LaunchPermissionModificationsTypeDef",
     "ImageDiskContainerTypeDef",
     "SnapshotDiskContainerTypeDef",
     "ListImagesInRecycleBinResultTypeDef",
     "ImportInstanceLaunchSpecificationTypeDef",
-    "InferenceAcceleratorInfoTypeDef",
+    "InferenceDeviceInfoTypeDef",
     "ModifyInstanceCreditSpecificationRequestRequestTypeDef",
     "LaunchTemplateInstanceNetworkInterfaceSpecificationRequestTypeDef",
     "ModifyInstanceMetadataOptionsResultTypeDef",
     "InstanceMonitoringTypeDef",
     "InstancePrivateIpAddressTypeDef",
     "InstanceRequirementsRequestTypeDef",
     "InstanceRequirementsTypeDef",
@@ -1903,22 +1908,22 @@
     "ValidationWarningTypeDef",
     "VerifiedAccessEndpointTypeDef",
     "VerifiedAccessInstanceTypeDef",
     "VerifiedAccessLogCloudWatchLogsDestinationTypeDef",
     "VerifiedAccessLogKinesisDataFirehoseDestinationTypeDef",
     "VerifiedAccessLogS3DestinationTypeDef",
     "VerifiedAccessLogOptionsTypeDef",
-    "VolumeResponseTypeDef",
-    "VolumeTypeDef",
     "VolumeStatusInfoTypeDef",
     "VpcCidrBlockAssociationTypeDef",
     "VpcIpv6CidrBlockAssociationTypeDef",
     "VpcPeeringConnectionVpcInfoResponseTypeDef",
     "VpcPeeringConnectionVpcInfoTypeDef",
     "LocalGatewayRouteTableTypeDef",
+    "VolumeResponseTypeDef",
+    "VolumeTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "AdditionalDetailTypeDef",
     "DescribeAddressesAttributeResultTypeDef",
     "ModifyAddressAttributeResultTypeDef",
     "ResetAddressAttributeResultTypeDef",
     "DescribeAddressesResultTypeDef",
     "DescribeVpcEndpointServicePermissionsResultTypeDef",
@@ -2172,14 +2177,15 @@
     "DisassociateIamInstanceProfileResultTypeDef",
     "ReplaceIamInstanceProfileAssociationResultTypeDef",
     "ModifyImageAttributeRequestImageModifyAttributeTypeDef",
     "ModifyImageAttributeRequestRequestTypeDef",
     "ImportImageRequestRequestTypeDef",
     "ImportSnapshotRequestRequestTypeDef",
     "ImportInstanceRequestRequestTypeDef",
+    "InferenceAcceleratorInfoTypeDef",
     "MonitorInstancesResultTypeDef",
     "UnmonitorInstancesResultTypeDef",
     "InstanceNetworkInterfaceTypeDef",
     "FleetLaunchTemplateOverridesRequestTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestGetInstanceTypesFromInstanceRequirementsPaginateTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestRequestTypeDef",
     "InstanceRequirementsWithMetadataRequestTypeDef",
@@ -2328,23 +2334,23 @@
     "CreateVerifiedAccessInstanceResultTypeDef",
     "DeleteVerifiedAccessInstanceResultTypeDef",
     "DescribeVerifiedAccessInstancesResultTypeDef",
     "DetachVerifiedAccessTrustProviderResultTypeDef",
     "ModifyVerifiedAccessInstanceResultTypeDef",
     "VerifiedAccessLogsTypeDef",
     "ModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef",
-    "DescribeVolumesResultTypeDef",
     "VolumeStatusItemTypeDef",
     "AssociateVpcCidrBlockResultTypeDef",
     "DisassociateVpcCidrBlockResultTypeDef",
     "VpcTypeDef",
     "VpcPeeringConnectionTypeDef",
     "CreateLocalGatewayRouteTableResultTypeDef",
     "DeleteLocalGatewayRouteTableResultTypeDef",
     "DescribeLocalGatewayRouteTablesResultTypeDef",
+    "DescribeVolumesResultTypeDef",
     "AssociateInstanceEventWindowResultTypeDef",
     "CreateInstanceEventWindowResultTypeDef",
     "DescribeInstanceEventWindowsResultTypeDef",
     "DisassociateInstanceEventWindowResultTypeDef",
     "ModifyInstanceEventWindowResultTypeDef",
     "PathComponentTypeDef",
     "CreateRouteTableResultTypeDef",
@@ -10138,20 +10144,18 @@
     "UserDataTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
 
-InferenceDeviceInfoTypeDef = TypedDict(
-    "InferenceDeviceInfoTypeDef",
+InferenceDeviceMemoryInfoTypeDef = TypedDict(
+    "InferenceDeviceMemoryInfoTypeDef",
     {
-        "Count": int,
-        "Name": str,
-        "Manufacturer": str,
+        "SizeInMiB": int,
     },
     total=False,
 )
 
 InstanceCountTypeDef = TypedDict(
     "InstanceCountTypeDef",
     {
@@ -10476,14 +10480,22 @@
     "MemoryInfoTypeDef",
     {
         "SizeInMiB": int,
     },
     total=False,
 )
 
+NitroTpmInfoTypeDef = TypedDict(
+    "NitroTpmInfoTypeDef",
+    {
+        "SupportedVersions": List[str],
+    },
+    total=False,
+)
+
 PlacementGroupInfoTypeDef = TypedDict(
     "PlacementGroupInfoTypeDef",
     {
         "SupportedStrategies": List[PlacementGroupStrategyType],
     },
     total=False,
 )
@@ -12007,14 +12019,16 @@
 
 NetworkCardInfoTypeDef = TypedDict(
     "NetworkCardInfoTypeDef",
     {
         "NetworkCardIndex": int,
         "NetworkPerformance": str,
         "MaximumNetworkInterfaces": int,
+        "BaselineBandwidthInGbps": float,
+        "PeakBandwidthInGbps": float,
     },
     total=False,
 )
 
 NetworkInterfaceAssociationTypeDef = TypedDict(
     "NetworkInterfaceAssociationTypeDef",
     {
@@ -13960,27 +13974,14 @@
         "Status": TelemetryStatusType,
         "StatusMessage": str,
         "CertificateArn": str,
     },
     total=False,
 )
 
-VolumeAttachmentTypeDef = TypedDict(
-    "VolumeAttachmentTypeDef",
-    {
-        "AttachTime": datetime,
-        "Device": str,
-        "InstanceId": str,
-        "State": VolumeAttachmentStateType,
-        "VolumeId": str,
-        "DeleteOnTermination": bool,
-    },
-    total=False,
-)
-
 VolumeStatusActionTypeDef = TypedDict(
     "VolumeStatusActionTypeDef",
     {
         "Code": str,
         "Description": str,
         "EventId": str,
         "EventType": str,
@@ -14629,14 +14630,15 @@
     },
 )
 
 GetEbsEncryptionByDefaultResultTypeDef = TypedDict(
     "GetEbsEncryptionByDefaultResultTypeDef",
     {
         "EbsEncryptionByDefault": bool,
+        "SseType": SSETypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFlowLogsIntegrationTemplateResultTypeDef = TypedDict(
     "GetFlowLogsIntegrationTemplateResultTypeDef",
     {
@@ -15090,14 +15092,15 @@
         "Encrypted": bool,
         "OwnerId": str,
         "Progress": str,
         "StartTime": datetime,
         "State": SnapshotStateType,
         "VolumeId": str,
         "VolumeSize": int,
+        "SseType": SSETypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreSnapshotTierResultTypeDef = TypedDict(
     "RestoreSnapshotTierResultTypeDef",
     {
@@ -15187,14 +15190,27 @@
         "State": VolumeAttachmentStateType,
         "VolumeId": str,
         "DeleteOnTermination": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+VolumeAttachmentTypeDef = TypedDict(
+    "VolumeAttachmentTypeDef",
+    {
+        "AttachTime": datetime,
+        "Device": str,
+        "InstanceId": str,
+        "State": VolumeAttachmentStateType,
+        "VolumeId": str,
+        "DeleteOnTermination": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VpcPeeringConnectionStateReasonResponseTypeDef = TypedDict(
     "VpcPeeringConnectionStateReasonResponseTypeDef",
     {
         "Code": VpcPeeringConnectionStateReasonCodeType,
         "Message": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -15838,14 +15854,15 @@
         "State": SnapshotStateType,
         "VolumeSize": int,
         "StartTime": datetime,
         "Progress": str,
         "OwnerId": str,
         "SnapshotId": str,
         "OutpostArn": str,
+        "SseType": SSETypeType,
     },
     total=False,
 )
 
 SnapshotResponseTypeDef = TypedDict(
     "SnapshotResponseTypeDef",
     {
@@ -15862,14 +15879,15 @@
         "VolumeId": str,
         "VolumeSize": int,
         "OwnerAlias": str,
         "OutpostArn": str,
         "Tags": List[TagTypeDef],
         "StorageTier": StorageTierType,
         "RestoreExpiryTime": datetime,
+        "SseType": SSETypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotTierStatusTypeDef = TypedDict(
     "SnapshotTierStatusTypeDef",
     {
@@ -15905,14 +15923,15 @@
         "VolumeId": str,
         "VolumeSize": int,
         "OwnerAlias": str,
         "OutpostArn": str,
         "Tags": List[TagTypeDef],
         "StorageTier": StorageTierType,
         "RestoreExpiryTime": datetime,
+        "SseType": SSETypeType,
     },
     total=False,
 )
 
 SpotFleetTagSpecificationTypeDef = TypedDict(
     "SpotFleetTagSpecificationTypeDef",
     {
@@ -22036,14 +22055,27 @@
         "NextToken": str,
         "MaxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeStoreImageTasksRequestStoreImageTaskCompleteWaitTypeDef = TypedDict(
+    "DescribeStoreImageTasksRequestStoreImageTaskCompleteWaitTypeDef",
+    {
+        "ImageIds": Sequence[str],
+        "DryRun": bool,
+        "Filters": Sequence[FilterTypeDef],
+        "NextToken": str,
+        "MaxResults": int,
+        "WaiterConfig": WaiterConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeSubnetsRequestSubnetAvailableWaitTypeDef = TypedDict(
     "DescribeSubnetsRequestSubnetAvailableWaitTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "SubnetIds": Sequence[str],
         "DryRun": bool,
         "NextToken": str,
@@ -23034,18 +23066,21 @@
         "PrivateIpAddress": str,
         "SubnetId": str,
         "UserData": UserDataTypeDef,
     },
     total=False,
 )
 
-InferenceAcceleratorInfoTypeDef = TypedDict(
-    "InferenceAcceleratorInfoTypeDef",
+InferenceDeviceInfoTypeDef = TypedDict(
+    "InferenceDeviceInfoTypeDef",
     {
-        "Accelerators": List[InferenceDeviceInfoTypeDef],
+        "Count": int,
+        "Name": str,
+        "Manufacturer": str,
+        "MemoryInfo": InferenceDeviceMemoryInfoTypeDef,
     },
     total=False,
 )
 
 _RequiredModifyInstanceCreditSpecificationRequestRequestTypeDef = TypedDict(
     "_RequiredModifyInstanceCreditSpecificationRequestRequestTypeDef",
     {
@@ -24612,60 +24647,14 @@
         "KinesisDataFirehose": VerifiedAccessLogKinesisDataFirehoseDestinationOptionsTypeDef,
         "LogVersion": str,
         "IncludeTrustContext": bool,
     },
     total=False,
 )
 
-VolumeResponseTypeDef = TypedDict(
-    "VolumeResponseTypeDef",
-    {
-        "Attachments": List[VolumeAttachmentTypeDef],
-        "AvailabilityZone": str,
-        "CreateTime": datetime,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "OutpostArn": str,
-        "Size": int,
-        "SnapshotId": str,
-        "State": VolumeStateType,
-        "VolumeId": str,
-        "Iops": int,
-        "Tags": List[TagTypeDef],
-        "VolumeType": VolumeTypeType,
-        "FastRestored": bool,
-        "MultiAttachEnabled": bool,
-        "Throughput": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-VolumeTypeDef = TypedDict(
-    "VolumeTypeDef",
-    {
-        "Attachments": List[VolumeAttachmentTypeDef],
-        "AvailabilityZone": str,
-        "CreateTime": datetime,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "OutpostArn": str,
-        "Size": int,
-        "SnapshotId": str,
-        "State": VolumeStateType,
-        "VolumeId": str,
-        "Iops": int,
-        "Tags": List[TagTypeDef],
-        "VolumeType": VolumeTypeType,
-        "FastRestored": bool,
-        "MultiAttachEnabled": bool,
-        "Throughput": int,
-    },
-    total=False,
-)
-
 VolumeStatusInfoTypeDef = TypedDict(
     "VolumeStatusInfoTypeDef",
     {
         "Details": List[VolumeStatusDetailsTypeDef],
         "Status": VolumeStatusInfoStatusType,
     },
     total=False,
@@ -24733,14 +24722,62 @@
         "Tags": List[TagTypeDef],
         "Mode": LocalGatewayRouteTableModeType,
         "StateReason": StateReasonTypeDef,
     },
     total=False,
 )
 
+VolumeResponseTypeDef = TypedDict(
+    "VolumeResponseTypeDef",
+    {
+        "Attachments": List[VolumeAttachmentTypeDef],
+        "AvailabilityZone": str,
+        "CreateTime": datetime,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "OutpostArn": str,
+        "Size": int,
+        "SnapshotId": str,
+        "State": VolumeStateType,
+        "VolumeId": str,
+        "Iops": int,
+        "Tags": List[TagTypeDef],
+        "VolumeType": VolumeTypeType,
+        "FastRestored": bool,
+        "MultiAttachEnabled": bool,
+        "Throughput": int,
+        "SseType": SSETypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VolumeTypeDef = TypedDict(
+    "VolumeTypeDef",
+    {
+        "Attachments": List[VolumeAttachmentTypeDef],
+        "AvailabilityZone": str,
+        "CreateTime": datetime,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "OutpostArn": str,
+        "Size": int,
+        "SnapshotId": str,
+        "State": VolumeStateType,
+        "VolumeId": str,
+        "Iops": int,
+        "Tags": List[TagTypeDef],
+        "VolumeType": VolumeTypeType,
+        "FastRestored": bool,
+        "MultiAttachEnabled": bool,
+        "Throughput": int,
+        "SseType": SSETypeType,
+    },
+    total=False,
+)
+
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -28997,14 +29034,23 @@
 
 class ImportInstanceRequestRequestTypeDef(
     _RequiredImportInstanceRequestRequestTypeDef, _OptionalImportInstanceRequestRequestTypeDef
 ):
     pass
 
 
+InferenceAcceleratorInfoTypeDef = TypedDict(
+    "InferenceAcceleratorInfoTypeDef",
+    {
+        "Accelerators": List[InferenceDeviceInfoTypeDef],
+        "TotalInferenceMemoryInMiB": int,
+    },
+    total=False,
+)
+
 MonitorInstancesResultTypeDef = TypedDict(
     "MonitorInstancesResultTypeDef",
     {
         "InstanceMonitorings": List[InstanceMonitoringTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -30753,23 +30799,14 @@
 class ModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef(
     _RequiredModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef,
     _OptionalModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeVolumesResultTypeDef = TypedDict(
-    "DescribeVolumesResultTypeDef",
-    {
-        "Volumes": List[VolumeTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 VolumeStatusItemTypeDef = TypedDict(
     "VolumeStatusItemTypeDef",
     {
         "Actions": List[VolumeStatusActionTypeDef],
         "AvailabilityZone": str,
         "OutpostArn": str,
         "Events": List[VolumeStatusEventTypeDef],
@@ -30851,14 +30888,23 @@
     {
         "LocalGatewayRouteTables": List[LocalGatewayRouteTableTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeVolumesResultTypeDef = TypedDict(
+    "DescribeVolumesResultTypeDef",
+    {
+        "Volumes": List[VolumeTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AssociateInstanceEventWindowResultTypeDef = TypedDict(
     "AssociateInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -31504,14 +31550,17 @@
         "PlacementGroupInfo": PlacementGroupInfoTypeDef,
         "InferenceAcceleratorInfo": InferenceAcceleratorInfoTypeDef,
         "HibernationSupported": bool,
         "BurstablePerformanceSupported": bool,
         "DedicatedHostsSupported": bool,
         "AutoRecoverySupported": bool,
         "SupportedBootModes": List[BootModeTypeType],
+        "NitroEnclavesSupport": NitroEnclavesSupportType,
+        "NitroTpmSupport": NitroTpmSupportType,
+        "NitroTpmInfo": NitroTpmInfoTypeDef,
     },
     total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/type_defs.pyi` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,16 @@
     NatGatewayAddressStatusType,
     NatGatewayStateType,
     NetworkInterfaceAttributeType,
     NetworkInterfaceCreationTypeType,
     NetworkInterfacePermissionStateCodeType,
     NetworkInterfaceStatusType,
     NetworkInterfaceTypeType,
+    NitroEnclavesSupportType,
+    NitroTpmSupportType,
     OfferingClassTypeType,
     OfferingTypeValuesType,
     OnDemandAllocationStrategyType,
     OperationTypeType,
     PartitionLoadFrequencyType,
     PaymentOptionType,
     PeriodTypeType,
@@ -226,14 +228,15 @@
     SnapshotAttributeNameType,
     SnapshotStateType,
     SpotAllocationStrategyType,
     SpotInstanceInterruptionBehaviorType,
     SpotInstanceStateType,
     SpotInstanceTypeType,
     SpreadLevelType,
+    SSETypeType,
     StateType,
     StaticSourcesSupportValueType,
     StatusType,
     StatusTypeType,
     StorageTierType,
     SubnetCidrBlockStateCodeType,
     SubnetCidrReservationTypeType,
@@ -809,15 +812,15 @@
     "LaunchPermissionTypeDef",
     "UserBucketTypeDef",
     "ImageRecycleBinInfoTypeDef",
     "ImportClientVpnClientCertificateRevocationListRequestRequestTypeDef",
     "ImportImageLicenseConfigurationRequestTypeDef",
     "ImportImageLicenseConfigurationResponseTypeDef",
     "UserDataTypeDef",
-    "InferenceDeviceInfoTypeDef",
+    "InferenceDeviceMemoryInfoTypeDef",
     "InstanceCountTypeDef",
     "InstanceCreditSpecificationRequestTypeDef",
     "InstanceEventWindowTimeRangeTypeDef",
     "InstanceIpv4PrefixTypeDef",
     "InstanceIpv6AddressRequestTypeDef",
     "InstanceIpv6PrefixTypeDef",
     "InstanceMaintenanceOptionsRequestTypeDef",
@@ -841,14 +844,15 @@
     "VCpuCountRangeTypeDef",
     "InstanceStateTypeDef",
     "InstanceStatusDetailsTypeDef",
     "InstanceStatusEventTypeDef",
     "LicenseConfigurationTypeDef",
     "PrivateDnsNameOptionsResponseTypeDef",
     "MemoryInfoTypeDef",
+    "NitroTpmInfoTypeDef",
     "PlacementGroupInfoTypeDef",
     "ProcessorInfoTypeDef",
     "VCpuInfoTypeDef",
     "IpRangeTypeDef",
     "Ipv6RangeTypeDef",
     "PrefixListIdTypeDef",
     "UserIdGroupPairTypeDef",
@@ -1086,15 +1090,14 @@
     "VerifiedAccessEndpointStatusTypeDef",
     "VerifiedAccessTrustProviderCondensedTypeDef",
     "VerifiedAccessLogCloudWatchLogsDestinationOptionsTypeDef",
     "VerifiedAccessLogDeliveryStatusTypeDef",
     "VerifiedAccessLogKinesisDataFirehoseDestinationOptionsTypeDef",
     "VerifiedAccessLogS3DestinationOptionsTypeDef",
     "VgwTelemetryTypeDef",
-    "VolumeAttachmentTypeDef",
     "VolumeStatusActionTypeDef",
     "VolumeStatusAttachmentStatusTypeDef",
     "VolumeStatusDetailsTypeDef",
     "VolumeStatusEventTypeDef",
     "VpcCidrBlockStateTypeDef",
     "VpcPeeringConnectionOptionsDescriptionTypeDef",
     "VpcPeeringConnectionStateReasonTypeDef",
@@ -1225,14 +1228,15 @@
     "StartVpcEndpointServicePrivateDnsVerificationResultTypeDef",
     "StateReasonResponseTypeDef",
     "StateReasonTypeDef",
     "UnassignIpv6AddressesResultTypeDef",
     "UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef",
     "UpdateSecurityGroupRuleDescriptionsIngressResultTypeDef",
     "VolumeAttachmentResponseTypeDef",
+    "VolumeAttachmentTypeDef",
     "VpcPeeringConnectionStateReasonResponseTypeDef",
     "AcceptReservedInstancesExchangeQuoteRequestRequestTypeDef",
     "GetReservedInstancesExchangeQuoteRequestRequestTypeDef",
     "AccountAttributeTypeDef",
     "DescribeFleetInstancesResultTypeDef",
     "DescribeSpotFleetInstancesResponseTypeDef",
     "ModifyVpcEndpointServicePermissionsResultTypeDef",
@@ -1719,14 +1723,15 @@
     "DescribeKeyPairsRequestKeyPairExistsWaitTypeDef",
     "DescribeNatGatewaysRequestNatGatewayAvailableWaitTypeDef",
     "DescribeNatGatewaysRequestNatGatewayDeletedWaitTypeDef",
     "DescribeNetworkInterfacesRequestNetworkInterfaceAvailableWaitTypeDef",
     "DescribeSecurityGroupsRequestSecurityGroupExistsWaitTypeDef",
     "DescribeSnapshotsRequestSnapshotCompletedWaitTypeDef",
     "DescribeSpotInstanceRequestsRequestSpotInstanceRequestFulfilledWaitTypeDef",
+    "DescribeStoreImageTasksRequestStoreImageTaskCompleteWaitTypeDef",
     "DescribeSubnetsRequestSubnetAvailableWaitTypeDef",
     "DescribeVolumesRequestVolumeAvailableWaitTypeDef",
     "DescribeVolumesRequestVolumeDeletedWaitTypeDef",
     "DescribeVolumesRequestVolumeInUseWaitTypeDef",
     "DescribeVpcPeeringConnectionsRequestVpcPeeringConnectionDeletedWaitTypeDef",
     "DescribeVpcPeeringConnectionsRequestVpcPeeringConnectionExistsWaitTypeDef",
     "DescribeVpcsRequestVpcAvailableWaitTypeDef",
@@ -1803,15 +1808,15 @@
     "GpuDeviceInfoTypeDef",
     "IamInstanceProfileAssociationTypeDef",
     "LaunchPermissionModificationsTypeDef",
     "ImageDiskContainerTypeDef",
     "SnapshotDiskContainerTypeDef",
     "ListImagesInRecycleBinResultTypeDef",
     "ImportInstanceLaunchSpecificationTypeDef",
-    "InferenceAcceleratorInfoTypeDef",
+    "InferenceDeviceInfoTypeDef",
     "ModifyInstanceCreditSpecificationRequestRequestTypeDef",
     "LaunchTemplateInstanceNetworkInterfaceSpecificationRequestTypeDef",
     "ModifyInstanceMetadataOptionsResultTypeDef",
     "InstanceMonitoringTypeDef",
     "InstancePrivateIpAddressTypeDef",
     "InstanceRequirementsRequestTypeDef",
     "InstanceRequirementsTypeDef",
@@ -1902,22 +1907,22 @@
     "ValidationWarningTypeDef",
     "VerifiedAccessEndpointTypeDef",
     "VerifiedAccessInstanceTypeDef",
     "VerifiedAccessLogCloudWatchLogsDestinationTypeDef",
     "VerifiedAccessLogKinesisDataFirehoseDestinationTypeDef",
     "VerifiedAccessLogS3DestinationTypeDef",
     "VerifiedAccessLogOptionsTypeDef",
-    "VolumeResponseTypeDef",
-    "VolumeTypeDef",
     "VolumeStatusInfoTypeDef",
     "VpcCidrBlockAssociationTypeDef",
     "VpcIpv6CidrBlockAssociationTypeDef",
     "VpcPeeringConnectionVpcInfoResponseTypeDef",
     "VpcPeeringConnectionVpcInfoTypeDef",
     "LocalGatewayRouteTableTypeDef",
+    "VolumeResponseTypeDef",
+    "VolumeTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "AdditionalDetailTypeDef",
     "DescribeAddressesAttributeResultTypeDef",
     "ModifyAddressAttributeResultTypeDef",
     "ResetAddressAttributeResultTypeDef",
     "DescribeAddressesResultTypeDef",
     "DescribeVpcEndpointServicePermissionsResultTypeDef",
@@ -2171,14 +2176,15 @@
     "DisassociateIamInstanceProfileResultTypeDef",
     "ReplaceIamInstanceProfileAssociationResultTypeDef",
     "ModifyImageAttributeRequestImageModifyAttributeTypeDef",
     "ModifyImageAttributeRequestRequestTypeDef",
     "ImportImageRequestRequestTypeDef",
     "ImportSnapshotRequestRequestTypeDef",
     "ImportInstanceRequestRequestTypeDef",
+    "InferenceAcceleratorInfoTypeDef",
     "MonitorInstancesResultTypeDef",
     "UnmonitorInstancesResultTypeDef",
     "InstanceNetworkInterfaceTypeDef",
     "FleetLaunchTemplateOverridesRequestTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestGetInstanceTypesFromInstanceRequirementsPaginateTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestRequestTypeDef",
     "InstanceRequirementsWithMetadataRequestTypeDef",
@@ -2327,23 +2333,23 @@
     "CreateVerifiedAccessInstanceResultTypeDef",
     "DeleteVerifiedAccessInstanceResultTypeDef",
     "DescribeVerifiedAccessInstancesResultTypeDef",
     "DetachVerifiedAccessTrustProviderResultTypeDef",
     "ModifyVerifiedAccessInstanceResultTypeDef",
     "VerifiedAccessLogsTypeDef",
     "ModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef",
-    "DescribeVolumesResultTypeDef",
     "VolumeStatusItemTypeDef",
     "AssociateVpcCidrBlockResultTypeDef",
     "DisassociateVpcCidrBlockResultTypeDef",
     "VpcTypeDef",
     "VpcPeeringConnectionTypeDef",
     "CreateLocalGatewayRouteTableResultTypeDef",
     "DeleteLocalGatewayRouteTableResultTypeDef",
     "DescribeLocalGatewayRouteTablesResultTypeDef",
+    "DescribeVolumesResultTypeDef",
     "AssociateInstanceEventWindowResultTypeDef",
     "CreateInstanceEventWindowResultTypeDef",
     "DescribeInstanceEventWindowsResultTypeDef",
     "DisassociateInstanceEventWindowResultTypeDef",
     "ModifyInstanceEventWindowResultTypeDef",
     "PathComponentTypeDef",
     "CreateRouteTableResultTypeDef",
@@ -9719,20 +9725,18 @@
     "UserDataTypeDef",
     {
         "Data": str,
     },
     total=False,
 )
 
-InferenceDeviceInfoTypeDef = TypedDict(
-    "InferenceDeviceInfoTypeDef",
+InferenceDeviceMemoryInfoTypeDef = TypedDict(
+    "InferenceDeviceMemoryInfoTypeDef",
     {
-        "Count": int,
-        "Name": str,
-        "Manufacturer": str,
+        "SizeInMiB": int,
     },
     total=False,
 )
 
 InstanceCountTypeDef = TypedDict(
     "InstanceCountTypeDef",
     {
@@ -10051,14 +10055,22 @@
     "MemoryInfoTypeDef",
     {
         "SizeInMiB": int,
     },
     total=False,
 )
 
+NitroTpmInfoTypeDef = TypedDict(
+    "NitroTpmInfoTypeDef",
+    {
+        "SupportedVersions": List[str],
+    },
+    total=False,
+)
+
 PlacementGroupInfoTypeDef = TypedDict(
     "PlacementGroupInfoTypeDef",
     {
         "SupportedStrategies": List[PlacementGroupStrategyType],
     },
     total=False,
 )
@@ -11516,14 +11528,16 @@
 
 NetworkCardInfoTypeDef = TypedDict(
     "NetworkCardInfoTypeDef",
     {
         "NetworkCardIndex": int,
         "NetworkPerformance": str,
         "MaximumNetworkInterfaces": int,
+        "BaselineBandwidthInGbps": float,
+        "PeakBandwidthInGbps": float,
     },
     total=False,
 )
 
 NetworkInterfaceAssociationTypeDef = TypedDict(
     "NetworkInterfaceAssociationTypeDef",
     {
@@ -13381,27 +13395,14 @@
         "Status": TelemetryStatusType,
         "StatusMessage": str,
         "CertificateArn": str,
     },
     total=False,
 )
 
-VolumeAttachmentTypeDef = TypedDict(
-    "VolumeAttachmentTypeDef",
-    {
-        "AttachTime": datetime,
-        "Device": str,
-        "InstanceId": str,
-        "State": VolumeAttachmentStateType,
-        "VolumeId": str,
-        "DeleteOnTermination": bool,
-    },
-    total=False,
-)
-
 VolumeStatusActionTypeDef = TypedDict(
     "VolumeStatusActionTypeDef",
     {
         "Code": str,
         "Description": str,
         "EventId": str,
         "EventType": str,
@@ -14048,14 +14049,15 @@
     },
 )
 
 GetEbsEncryptionByDefaultResultTypeDef = TypedDict(
     "GetEbsEncryptionByDefaultResultTypeDef",
     {
         "EbsEncryptionByDefault": bool,
+        "SseType": SSETypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFlowLogsIntegrationTemplateResultTypeDef = TypedDict(
     "GetFlowLogsIntegrationTemplateResultTypeDef",
     {
@@ -14509,14 +14511,15 @@
         "Encrypted": bool,
         "OwnerId": str,
         "Progress": str,
         "StartTime": datetime,
         "State": SnapshotStateType,
         "VolumeId": str,
         "VolumeSize": int,
+        "SseType": SSETypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreSnapshotTierResultTypeDef = TypedDict(
     "RestoreSnapshotTierResultTypeDef",
     {
@@ -14606,14 +14609,27 @@
         "State": VolumeAttachmentStateType,
         "VolumeId": str,
         "DeleteOnTermination": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+VolumeAttachmentTypeDef = TypedDict(
+    "VolumeAttachmentTypeDef",
+    {
+        "AttachTime": datetime,
+        "Device": str,
+        "InstanceId": str,
+        "State": VolumeAttachmentStateType,
+        "VolumeId": str,
+        "DeleteOnTermination": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VpcPeeringConnectionStateReasonResponseTypeDef = TypedDict(
     "VpcPeeringConnectionStateReasonResponseTypeDef",
     {
         "Code": VpcPeeringConnectionStateReasonCodeType,
         "Message": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -15245,14 +15261,15 @@
         "State": SnapshotStateType,
         "VolumeSize": int,
         "StartTime": datetime,
         "Progress": str,
         "OwnerId": str,
         "SnapshotId": str,
         "OutpostArn": str,
+        "SseType": SSETypeType,
     },
     total=False,
 )
 
 SnapshotResponseTypeDef = TypedDict(
     "SnapshotResponseTypeDef",
     {
@@ -15269,14 +15286,15 @@
         "VolumeId": str,
         "VolumeSize": int,
         "OwnerAlias": str,
         "OutpostArn": str,
         "Tags": List[TagTypeDef],
         "StorageTier": StorageTierType,
         "RestoreExpiryTime": datetime,
+        "SseType": SSETypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotTierStatusTypeDef = TypedDict(
     "SnapshotTierStatusTypeDef",
     {
@@ -15312,14 +15330,15 @@
         "VolumeId": str,
         "VolumeSize": int,
         "OwnerAlias": str,
         "OutpostArn": str,
         "Tags": List[TagTypeDef],
         "StorageTier": StorageTierType,
         "RestoreExpiryTime": datetime,
+        "SseType": SSETypeType,
     },
     total=False,
 )
 
 SpotFleetTagSpecificationTypeDef = TypedDict(
     "SpotFleetTagSpecificationTypeDef",
     {
@@ -21293,14 +21312,27 @@
         "NextToken": str,
         "MaxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeStoreImageTasksRequestStoreImageTaskCompleteWaitTypeDef = TypedDict(
+    "DescribeStoreImageTasksRequestStoreImageTaskCompleteWaitTypeDef",
+    {
+        "ImageIds": Sequence[str],
+        "DryRun": bool,
+        "Filters": Sequence[FilterTypeDef],
+        "NextToken": str,
+        "MaxResults": int,
+        "WaiterConfig": WaiterConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeSubnetsRequestSubnetAvailableWaitTypeDef = TypedDict(
     "DescribeSubnetsRequestSubnetAvailableWaitTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "SubnetIds": Sequence[str],
         "DryRun": bool,
         "NextToken": str,
@@ -22283,18 +22315,21 @@
         "PrivateIpAddress": str,
         "SubnetId": str,
         "UserData": UserDataTypeDef,
     },
     total=False,
 )
 
-InferenceAcceleratorInfoTypeDef = TypedDict(
-    "InferenceAcceleratorInfoTypeDef",
+InferenceDeviceInfoTypeDef = TypedDict(
+    "InferenceDeviceInfoTypeDef",
     {
-        "Accelerators": List[InferenceDeviceInfoTypeDef],
+        "Count": int,
+        "Name": str,
+        "Manufacturer": str,
+        "MemoryInfo": InferenceDeviceMemoryInfoTypeDef,
     },
     total=False,
 )
 
 _RequiredModifyInstanceCreditSpecificationRequestRequestTypeDef = TypedDict(
     "_RequiredModifyInstanceCreditSpecificationRequestRequestTypeDef",
     {
@@ -23829,60 +23864,14 @@
         "KinesisDataFirehose": VerifiedAccessLogKinesisDataFirehoseDestinationOptionsTypeDef,
         "LogVersion": str,
         "IncludeTrustContext": bool,
     },
     total=False,
 )
 
-VolumeResponseTypeDef = TypedDict(
-    "VolumeResponseTypeDef",
-    {
-        "Attachments": List[VolumeAttachmentTypeDef],
-        "AvailabilityZone": str,
-        "CreateTime": datetime,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "OutpostArn": str,
-        "Size": int,
-        "SnapshotId": str,
-        "State": VolumeStateType,
-        "VolumeId": str,
-        "Iops": int,
-        "Tags": List[TagTypeDef],
-        "VolumeType": VolumeTypeType,
-        "FastRestored": bool,
-        "MultiAttachEnabled": bool,
-        "Throughput": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-VolumeTypeDef = TypedDict(
-    "VolumeTypeDef",
-    {
-        "Attachments": List[VolumeAttachmentTypeDef],
-        "AvailabilityZone": str,
-        "CreateTime": datetime,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "OutpostArn": str,
-        "Size": int,
-        "SnapshotId": str,
-        "State": VolumeStateType,
-        "VolumeId": str,
-        "Iops": int,
-        "Tags": List[TagTypeDef],
-        "VolumeType": VolumeTypeType,
-        "FastRestored": bool,
-        "MultiAttachEnabled": bool,
-        "Throughput": int,
-    },
-    total=False,
-)
-
 VolumeStatusInfoTypeDef = TypedDict(
     "VolumeStatusInfoTypeDef",
     {
         "Details": List[VolumeStatusDetailsTypeDef],
         "Status": VolumeStatusInfoStatusType,
     },
     total=False,
@@ -23950,14 +23939,62 @@
         "Tags": List[TagTypeDef],
         "Mode": LocalGatewayRouteTableModeType,
         "StateReason": StateReasonTypeDef,
     },
     total=False,
 )
 
+VolumeResponseTypeDef = TypedDict(
+    "VolumeResponseTypeDef",
+    {
+        "Attachments": List[VolumeAttachmentTypeDef],
+        "AvailabilityZone": str,
+        "CreateTime": datetime,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "OutpostArn": str,
+        "Size": int,
+        "SnapshotId": str,
+        "State": VolumeStateType,
+        "VolumeId": str,
+        "Iops": int,
+        "Tags": List[TagTypeDef],
+        "VolumeType": VolumeTypeType,
+        "FastRestored": bool,
+        "MultiAttachEnabled": bool,
+        "Throughput": int,
+        "SseType": SSETypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VolumeTypeDef = TypedDict(
+    "VolumeTypeDef",
+    {
+        "Attachments": List[VolumeAttachmentTypeDef],
+        "AvailabilityZone": str,
+        "CreateTime": datetime,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "OutpostArn": str,
+        "Size": int,
+        "SnapshotId": str,
+        "State": VolumeStateType,
+        "VolumeId": str,
+        "Iops": int,
+        "Tags": List[TagTypeDef],
+        "VolumeType": VolumeTypeType,
+        "FastRestored": bool,
+        "MultiAttachEnabled": bool,
+        "Throughput": int,
+        "SseType": SSETypeType,
+    },
+    total=False,
+)
+
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -28044,14 +28081,23 @@
 )
 
 class ImportInstanceRequestRequestTypeDef(
     _RequiredImportInstanceRequestRequestTypeDef, _OptionalImportInstanceRequestRequestTypeDef
 ):
     pass
 
+InferenceAcceleratorInfoTypeDef = TypedDict(
+    "InferenceAcceleratorInfoTypeDef",
+    {
+        "Accelerators": List[InferenceDeviceInfoTypeDef],
+        "TotalInferenceMemoryInMiB": int,
+    },
+    total=False,
+)
+
 MonitorInstancesResultTypeDef = TypedDict(
     "MonitorInstancesResultTypeDef",
     {
         "InstanceMonitorings": List[InstanceMonitoringTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -29782,23 +29828,14 @@
 
 class ModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef(
     _RequiredModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef,
     _OptionalModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef,
 ):
     pass
 
-DescribeVolumesResultTypeDef = TypedDict(
-    "DescribeVolumesResultTypeDef",
-    {
-        "Volumes": List[VolumeTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 VolumeStatusItemTypeDef = TypedDict(
     "VolumeStatusItemTypeDef",
     {
         "Actions": List[VolumeStatusActionTypeDef],
         "AvailabilityZone": str,
         "OutpostArn": str,
         "Events": List[VolumeStatusEventTypeDef],
@@ -29880,14 +29917,23 @@
     {
         "LocalGatewayRouteTables": List[LocalGatewayRouteTableTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeVolumesResultTypeDef = TypedDict(
+    "DescribeVolumesResultTypeDef",
+    {
+        "Volumes": List[VolumeTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AssociateInstanceEventWindowResultTypeDef = TypedDict(
     "AssociateInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -30521,14 +30567,17 @@
         "PlacementGroupInfo": PlacementGroupInfoTypeDef,
         "InferenceAcceleratorInfo": InferenceAcceleratorInfoTypeDef,
         "HibernationSupported": bool,
         "BurstablePerformanceSupported": bool,
         "DedicatedHostsSupported": bool,
         "AutoRecoverySupported": bool,
         "SupportedBootModes": List[BootModeTypeType],
+        "NitroEnclavesSupport": NitroEnclavesSupportType,
+        "NitroTpmSupport": NitroTpmSupportType,
+        "NitroTpmInfo": NitroTpmInfoTypeDef,
     },
     total=False,
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/waiter.py` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         NatGatewayDeletedWaiter,
         NetworkInterfaceAvailableWaiter,
         PasswordDataAvailableWaiter,
         SecurityGroupExistsWaiter,
         SnapshotCompletedWaiter,
         SnapshotImportedWaiter,
         SpotInstanceRequestFulfilledWaiter,
+        StoreImageTaskCompleteWaiter,
         SubnetAvailableWaiter,
         SystemStatusOkWaiter,
         VolumeAvailableWaiter,
         VolumeDeletedWaiter,
         VolumeInUseWaiter,
         VpcAvailableWaiter,
         VpcExistsWaiter,
@@ -71,14 +72,15 @@
         nat_gateway_deleted_waiter: NatGatewayDeletedWaiter = client.get_waiter("nat_gateway_deleted")
         network_interface_available_waiter: NetworkInterfaceAvailableWaiter = client.get_waiter("network_interface_available")
         password_data_available_waiter: PasswordDataAvailableWaiter = client.get_waiter("password_data_available")
         security_group_exists_waiter: SecurityGroupExistsWaiter = client.get_waiter("security_group_exists")
         snapshot_completed_waiter: SnapshotCompletedWaiter = client.get_waiter("snapshot_completed")
         snapshot_imported_waiter: SnapshotImportedWaiter = client.get_waiter("snapshot_imported")
         spot_instance_request_fulfilled_waiter: SpotInstanceRequestFulfilledWaiter = client.get_waiter("spot_instance_request_fulfilled")
+        store_image_task_complete_waiter: StoreImageTaskCompleteWaiter = client.get_waiter("store_image_task_complete")
         subnet_available_waiter: SubnetAvailableWaiter = client.get_waiter("subnet_available")
         system_status_ok_waiter: SystemStatusOkWaiter = client.get_waiter("system_status_ok")
         volume_available_waiter: VolumeAvailableWaiter = client.get_waiter("volume_available")
         volume_deleted_waiter: VolumeDeletedWaiter = client.get_waiter("volume_deleted")
         volume_in_use_waiter: VolumeInUseWaiter = client.get_waiter("volume_in_use")
         vpc_available_waiter: VpcAvailableWaiter = client.get_waiter("vpc_available")
         vpc_exists_waiter: VpcExistsWaiter = client.get_waiter("vpc_exists")
@@ -115,14 +117,15 @@
     "NatGatewayDeletedWaiter",
     "NetworkInterfaceAvailableWaiter",
     "PasswordDataAvailableWaiter",
     "SecurityGroupExistsWaiter",
     "SnapshotCompletedWaiter",
     "SnapshotImportedWaiter",
     "SpotInstanceRequestFulfilledWaiter",
+    "StoreImageTaskCompleteWaiter",
     "SubnetAvailableWaiter",
     "SystemStatusOkWaiter",
     "VolumeAvailableWaiter",
     "VolumeDeletedWaiter",
     "VolumeInUseWaiter",
     "VpcAvailableWaiter",
     "VpcExistsWaiter",
@@ -641,14 +644,36 @@
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Waiter.SpotInstanceRequestFulfilled.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/waiters/#spotinstancerequestfulfilledwaiter)
         """
 
 
+class StoreImageTaskCompleteWaiter(AIOWaiter):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Waiter.StoreImageTaskComplete)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/waiters/#storeimagetaskcompletewaiter)
+    """
+
+    async def wait(
+        self,
+        *,
+        ImageIds: Sequence[str] = ...,
+        DryRun: bool = ...,
+        Filters: Sequence[FilterTypeDef] = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        WaiterConfig: WaiterConfigTypeDef = ...
+    ) -> None:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Waiter.StoreImageTaskComplete.wait)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/waiters/#storeimagetaskcompletewaiter)
+        """
+
+
 class SubnetAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Waiter.SubnetAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/waiters/#subnetavailablewaiter)
     """
 
     async def wait(
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2/waiter.pyi` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         NatGatewayDeletedWaiter,
         NetworkInterfaceAvailableWaiter,
         PasswordDataAvailableWaiter,
         SecurityGroupExistsWaiter,
         SnapshotCompletedWaiter,
         SnapshotImportedWaiter,
         SpotInstanceRequestFulfilledWaiter,
+        StoreImageTaskCompleteWaiter,
         SubnetAvailableWaiter,
         SystemStatusOkWaiter,
         VolumeAvailableWaiter,
         VolumeDeletedWaiter,
         VolumeInUseWaiter,
         VpcAvailableWaiter,
         VpcExistsWaiter,
@@ -71,14 +72,15 @@
         nat_gateway_deleted_waiter: NatGatewayDeletedWaiter = client.get_waiter("nat_gateway_deleted")
         network_interface_available_waiter: NetworkInterfaceAvailableWaiter = client.get_waiter("network_interface_available")
         password_data_available_waiter: PasswordDataAvailableWaiter = client.get_waiter("password_data_available")
         security_group_exists_waiter: SecurityGroupExistsWaiter = client.get_waiter("security_group_exists")
         snapshot_completed_waiter: SnapshotCompletedWaiter = client.get_waiter("snapshot_completed")
         snapshot_imported_waiter: SnapshotImportedWaiter = client.get_waiter("snapshot_imported")
         spot_instance_request_fulfilled_waiter: SpotInstanceRequestFulfilledWaiter = client.get_waiter("spot_instance_request_fulfilled")
+        store_image_task_complete_waiter: StoreImageTaskCompleteWaiter = client.get_waiter("store_image_task_complete")
         subnet_available_waiter: SubnetAvailableWaiter = client.get_waiter("subnet_available")
         system_status_ok_waiter: SystemStatusOkWaiter = client.get_waiter("system_status_ok")
         volume_available_waiter: VolumeAvailableWaiter = client.get_waiter("volume_available")
         volume_deleted_waiter: VolumeDeletedWaiter = client.get_waiter("volume_deleted")
         volume_in_use_waiter: VolumeInUseWaiter = client.get_waiter("volume_in_use")
         vpc_available_waiter: VpcAvailableWaiter = client.get_waiter("vpc_available")
         vpc_exists_waiter: VpcExistsWaiter = client.get_waiter("vpc_exists")
@@ -115,14 +117,15 @@
     "NatGatewayDeletedWaiter",
     "NetworkInterfaceAvailableWaiter",
     "PasswordDataAvailableWaiter",
     "SecurityGroupExistsWaiter",
     "SnapshotCompletedWaiter",
     "SnapshotImportedWaiter",
     "SpotInstanceRequestFulfilledWaiter",
+    "StoreImageTaskCompleteWaiter",
     "SubnetAvailableWaiter",
     "SystemStatusOkWaiter",
     "VolumeAvailableWaiter",
     "VolumeDeletedWaiter",
     "VolumeInUseWaiter",
     "VpcAvailableWaiter",
     "VpcExistsWaiter",
@@ -616,14 +619,35 @@
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Waiter.SpotInstanceRequestFulfilled.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/waiters/#spotinstancerequestfulfilledwaiter)
         """
 
+class StoreImageTaskCompleteWaiter(AIOWaiter):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Waiter.StoreImageTaskComplete)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/waiters/#storeimagetaskcompletewaiter)
+    """
+
+    async def wait(
+        self,
+        *,
+        ImageIds: Sequence[str] = ...,
+        DryRun: bool = ...,
+        Filters: Sequence[FilterTypeDef] = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        WaiterConfig: WaiterConfigTypeDef = ...
+    ) -> None:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Waiter.StoreImageTaskComplete.wait)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/waiters/#storeimagetaskcompletewaiter)
+        """
+
 class SubnetAvailableWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Waiter.SubnetAvailable)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/waiters/#subnetavailablewaiter)
     """
 
     async def wait(
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2.egg-info/PKG-INFO` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.EC2 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.EC2 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ec2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ec2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ec2)](https://pepy.tech/project/types-aiobotocore-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EC2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[aiobotocore.EC2 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -856,14 +856,15 @@
     NatGatewayDeletedWaiter,
     NetworkInterfaceAvailableWaiter,
     PasswordDataAvailableWaiter,
     SecurityGroupExistsWaiter,
     SnapshotCompletedWaiter,
     SnapshotImportedWaiter,
     SpotInstanceRequestFulfilledWaiter,
+    StoreImageTaskCompleteWaiter,
     SubnetAvailableWaiter,
     SystemStatusOkWaiter,
     VolumeAvailableWaiter,
     VolumeDeletedWaiter,
     VolumeInUseWaiter,
     VpcAvailableWaiter,
     VpcExistsWaiter,
@@ -925,14 +926,17 @@
         "security_group_exists"
     )
     snapshot_completed_waiter: SnapshotCompletedWaiter = client.get_waiter("snapshot_completed")
     snapshot_imported_waiter: SnapshotImportedWaiter = client.get_waiter("snapshot_imported")
     spot_instance_request_fulfilled_waiter: SpotInstanceRequestFulfilledWaiter = client.get_waiter(
         "spot_instance_request_fulfilled"
     )
+    store_image_task_complete_waiter: StoreImageTaskCompleteWaiter = client.get_waiter(
+        "store_image_task_complete"
+    )
     subnet_available_waiter: SubnetAvailableWaiter = client.get_waiter("subnet_available")
     system_status_ok_waiter: SystemStatusOkWaiter = client.get_waiter("system_status_ok")
     volume_available_waiter: VolumeAvailableWaiter = client.get_waiter("volume_available")
     volume_deleted_waiter: VolumeDeletedWaiter = client.get_waiter("volume_deleted")
     volume_in_use_waiter: VolumeInUseWaiter = client.get_waiter("volume_in_use")
     vpc_available_waiter: VpcAvailableWaiter = client.get_waiter("vpc_available")
     vpc_exists_waiter: VpcExistsWaiter = client.get_waiter("vpc_exists")
```

### Comparing `types-aiobotocore-ec2-2.5.2.post3/types_aiobotocore_ec2.egg-info/SOURCES.txt` & `types-aiobotocore-ec2-2.5.4/types_aiobotocore_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

