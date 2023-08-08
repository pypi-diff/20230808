# Comparing `tmp/types-aiobotocore-autoscaling-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-autoscaling-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-autoscaling-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-autoscaling-2.5.4.tar", last modified: Tue Aug  8 01:23:21 2023, max compression
```

## Comparing `types-aiobotocore-autoscaling-2.5.2.post3.tar` & `types-aiobotocore-autoscaling-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:19.027228 types-aiobotocore-autoscaling-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:18:47.000000 types-aiobotocore-autoscaling-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-08-04 12:37:19.023228 types-aiobotocore-autoscaling-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-08-04 12:18:47.000000 types-aiobotocore-autoscaling-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:19.027228 types-aiobotocore-autoscaling-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-04 12:18:47.000000 types-aiobotocore-autoscaling-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:19.015228 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-08-04 12:18:47.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-08-04 12:18:47.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-04 12:18:47.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55187 2023-08-04 12:18:47.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    55103 2023-08-04 12:18:47.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-08-04 12:18:48.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-08-04 12:18:48.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-08-04 12:18:48.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-08-04 12:18:48.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:18:47.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75359 2023-08-04 12:18:50.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75242 2023-08-04 12:18:49.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:18:47.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:19.023228 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 12:37:18.000000 types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.526620 types-aiobotocore-autoscaling-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-08-08 01:23:21.526620 types-aiobotocore-autoscaling-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:21.526620 types-aiobotocore-autoscaling-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.522620 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55680 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55595 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14949 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14936 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    76252 2023-08-08 01:06:36.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76133 2023-08-08 01:06:35.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:06:34.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:21.526620 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 01:23:21.000000 types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/LICENSE` & `types-aiobotocore-autoscaling-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/PKG-INFO` & `types-aiobotocore-autoscaling-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AutoScaling 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AutoScaling 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling)](https://pepy.tech/project/types-aiobotocore-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[aiobotocore.AutoScaling 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -282,14 +282,15 @@
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeLoadBalancersPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 
 session = get_session()
 async with session.create_client("autoscaling") as client:
     client: AutoScalingClient
 
     # Explicit type annotations are optional here
@@ -318,14 +319,17 @@
     describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = (
         client.get_paginator("describe_scaling_activities")
     )
     describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator(
         "describe_scheduled_actions"
     )
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+    describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator(
+        "describe_warm_pool"
+    )
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_autoscaling.literals` module contains literals extracted
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/README.md` & `types-aiobotocore-autoscaling-2.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling)](https://pepy.tech/project/types-aiobotocore-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[aiobotocore.AutoScaling 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -250,14 +250,15 @@
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeLoadBalancersPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 
 session = get_session()
 async with session.create_client("autoscaling") as client:
     client: AutoScalingClient
 
     # Explicit type annotations are optional here
@@ -286,14 +287,17 @@
     describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = (
         client.get_paginator("describe_scaling_activities")
     )
     describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator(
         "describe_scheduled_actions"
     )
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+    describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator(
+        "describe_warm_pool"
+    )
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_autoscaling.literals` module contains literals extracted
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/setup.py` & `types-aiobotocore-autoscaling-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-autoscaling",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AutoScaling 2.5.2 service generated with"
+        "Type annotations for aiobotocore.AutoScaling 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/__init__.py` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         DescribeLoadBalancerTargetGroupsPaginator,
         DescribeLoadBalancersPaginator,
         DescribeNotificationConfigurationsPaginator,
         DescribePoliciesPaginator,
         DescribeScalingActivitiesPaginator,
         DescribeScheduledActionsPaginator,
         DescribeTagsPaginator,
+        DescribeWarmPoolPaginator,
     )
 
     session = get_session()
     async with session.create_client("autoscaling") as client:
         client: AutoScalingClient
         ...
 
@@ -32,28 +33,30 @@
     describe_load_balancer_target_groups_paginator: DescribeLoadBalancerTargetGroupsPaginator = client.get_paginator("describe_load_balancer_target_groups")
     describe_load_balancers_paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
     describe_notification_configurations_paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")
     describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
     describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
     describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+    describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
     ```
 """
 from .client import AutoScalingClient
 from .paginator import (
     DescribeAutoScalingGroupsPaginator,
     DescribeAutoScalingInstancesPaginator,
     DescribeLaunchConfigurationsPaginator,
     DescribeLoadBalancersPaginator,
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 
 Client = AutoScalingClient
 
 
 __all__ = (
     "AutoScalingClient",
@@ -64,8 +67,9 @@
     "DescribeLoadBalancerTargetGroupsPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeNotificationConfigurationsPaginator",
     "DescribePoliciesPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScheduledActionsPaginator",
     "DescribeTagsPaginator",
+    "DescribeWarmPoolPaginator",
 )
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/__init__.pyi` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         DescribeLoadBalancerTargetGroupsPaginator,
         DescribeLoadBalancersPaginator,
         DescribeNotificationConfigurationsPaginator,
         DescribePoliciesPaginator,
         DescribeScalingActivitiesPaginator,
         DescribeScheduledActionsPaginator,
         DescribeTagsPaginator,
+        DescribeWarmPoolPaginator,
     )
 
     session = get_session()
     async with session.create_client("autoscaling") as client:
         client: AutoScalingClient
         ...
 
@@ -32,28 +33,30 @@
     describe_load_balancer_target_groups_paginator: DescribeLoadBalancerTargetGroupsPaginator = client.get_paginator("describe_load_balancer_target_groups")
     describe_load_balancers_paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
     describe_notification_configurations_paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")
     describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
     describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
     describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+    describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
     ```
 """
 from .client import AutoScalingClient
 from .paginator import (
     DescribeAutoScalingGroupsPaginator,
     DescribeAutoScalingInstancesPaginator,
     DescribeLaunchConfigurationsPaginator,
     DescribeLoadBalancersPaginator,
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 
 Client = AutoScalingClient
 
 __all__ = (
     "AutoScalingClient",
     "Client",
@@ -63,8 +66,9 @@
     "DescribeLoadBalancerTargetGroupsPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeNotificationConfigurationsPaginator",
     "DescribePoliciesPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScheduledActionsPaginator",
     "DescribeTagsPaginator",
+    "DescribeWarmPoolPaginator",
 )
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/__main__.py` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AutoScaling 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        "Type annotations for aiobotocore.AutoScaling 2.5.4\nVersion:         2.5.4\nBuilder"
         " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
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

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/client.py` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     DescribeLoadBalancersPaginator,
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 from .type_defs import (
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
@@ -895,15 +896,15 @@
         process, for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.resume_processes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#resume_processes)
         """
 
     async def rollback_instance_refresh(
-        self, *, AutoScalingGroupName: str = ...
+        self, *, AutoScalingGroupName: str
     ) -> RollbackInstanceRefreshAnswerTypeDef:
         """
         Cancels an instance refresh that is in progress and rolls back any changes that
         it made.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.rollback_instance_refresh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#rollback_instance_refresh)
@@ -1093,14 +1094,23 @@
     @overload
     def get_paginator(self, operation_name: Literal["describe_tags"]) -> DescribeTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#get_paginator)
         """
 
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_warm_pool"]
+    ) -> DescribeWarmPoolPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#get_paginator)
+        """
+
     async def __aenter__(self) -> "AutoScalingClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/)
         """
 
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/client.pyi` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     DescribeLoadBalancersPaginator,
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 from .type_defs import (
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
@@ -830,15 +831,15 @@
         Resumes the specified suspended auto scaling processes, or all suspended
         process, for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.resume_processes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#resume_processes)
         """
     async def rollback_instance_refresh(
-        self, *, AutoScalingGroupName: str = ...
+        self, *, AutoScalingGroupName: str
     ) -> RollbackInstanceRefreshAnswerTypeDef:
         """
         Cancels an instance refresh that is in progress and rolls back any changes that
         it made.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.rollback_instance_refresh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#rollback_instance_refresh)
@@ -1010,14 +1011,22 @@
         """
     @overload
     def get_paginator(self, operation_name: Literal["describe_tags"]) -> DescribeTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#get_paginator)
         """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_warm_pool"]
+    ) -> DescribeWarmPoolPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#get_paginator)
+        """
     async def __aenter__(self) -> "AutoScalingClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/)
         """
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/literals.py` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "DescribeLoadBalancerTargetGroupsPaginatorName",
     "DescribeLoadBalancersPaginatorName",
     "DescribeNotificationConfigurationsPaginatorName",
     "DescribePoliciesPaginatorName",
     "DescribeScalingActivitiesPaginatorName",
     "DescribeScheduledActionsPaginatorName",
     "DescribeTagsPaginatorName",
+    "DescribeWarmPoolPaginatorName",
     "InstanceGenerationType",
     "InstanceMetadataEndpointStateType",
     "InstanceMetadataHttpTokensStateType",
     "InstanceRefreshStatusType",
     "LifecycleStateType",
     "LocalStorageType",
     "LocalStorageTypeType",
@@ -76,14 +77,15 @@
 DescribeLoadBalancerTargetGroupsPaginatorName = Literal["describe_load_balancer_target_groups"]
 DescribeLoadBalancersPaginatorName = Literal["describe_load_balancers"]
 DescribeNotificationConfigurationsPaginatorName = Literal["describe_notification_configurations"]
 DescribePoliciesPaginatorName = Literal["describe_policies"]
 DescribeScalingActivitiesPaginatorName = Literal["describe_scaling_activities"]
 DescribeScheduledActionsPaginatorName = Literal["describe_scheduled_actions"]
 DescribeTagsPaginatorName = Literal["describe_tags"]
+DescribeWarmPoolPaginatorName = Literal["describe_warm_pool"]
 InstanceGenerationType = Literal["current", "previous"]
 InstanceMetadataEndpointStateType = Literal["disabled", "enabled"]
 InstanceMetadataHttpTokensStateType = Literal["optional", "required"]
 InstanceRefreshStatusType = Literal[
     "Cancelled",
     "Cancelling",
     "Failed",
@@ -177,14 +179,15 @@
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
@@ -280,14 +283,15 @@
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
@@ -366,26 +370,28 @@
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
@@ -536,14 +542,15 @@
     "describe_load_balancer_target_groups",
     "describe_load_balancers",
     "describe_notification_configurations",
     "describe_policies",
     "describe_scaling_activities",
     "describe_scheduled_actions",
     "describe_tags",
+    "describe_warm_pool",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
@@ -558,14 +565,15 @@
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

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/literals.pyi` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "DescribeLoadBalancerTargetGroupsPaginatorName",
     "DescribeLoadBalancersPaginatorName",
     "DescribeNotificationConfigurationsPaginatorName",
     "DescribePoliciesPaginatorName",
     "DescribeScalingActivitiesPaginatorName",
     "DescribeScheduledActionsPaginatorName",
     "DescribeTagsPaginatorName",
+    "DescribeWarmPoolPaginatorName",
     "InstanceGenerationType",
     "InstanceMetadataEndpointStateType",
     "InstanceMetadataHttpTokensStateType",
     "InstanceRefreshStatusType",
     "LifecycleStateType",
     "LocalStorageType",
     "LocalStorageTypeType",
@@ -74,14 +75,15 @@
 DescribeLoadBalancerTargetGroupsPaginatorName = Literal["describe_load_balancer_target_groups"]
 DescribeLoadBalancersPaginatorName = Literal["describe_load_balancers"]
 DescribeNotificationConfigurationsPaginatorName = Literal["describe_notification_configurations"]
 DescribePoliciesPaginatorName = Literal["describe_policies"]
 DescribeScalingActivitiesPaginatorName = Literal["describe_scaling_activities"]
 DescribeScheduledActionsPaginatorName = Literal["describe_scheduled_actions"]
 DescribeTagsPaginatorName = Literal["describe_tags"]
+DescribeWarmPoolPaginatorName = Literal["describe_warm_pool"]
 InstanceGenerationType = Literal["current", "previous"]
 InstanceMetadataEndpointStateType = Literal["disabled", "enabled"]
 InstanceMetadataHttpTokensStateType = Literal["optional", "required"]
 InstanceRefreshStatusType = Literal[
     "Cancelled",
     "Cancelling",
     "Failed",
@@ -175,14 +177,15 @@
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
@@ -278,14 +281,15 @@
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
@@ -364,26 +368,28 @@
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
@@ -534,14 +540,15 @@
     "describe_load_balancer_target_groups",
     "describe_load_balancers",
     "describe_notification_configurations",
     "describe_policies",
     "describe_scaling_activities",
     "describe_scheduled_actions",
     "describe_tags",
+    "describe_warm_pool",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
@@ -556,14 +563,15 @@
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

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/paginator.py` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         DescribeLoadBalancerTargetGroupsPaginator,
         DescribeLoadBalancersPaginator,
         DescribeNotificationConfigurationsPaginator,
         DescribePoliciesPaginator,
         DescribeScalingActivitiesPaginator,
         DescribeScheduledActionsPaginator,
         DescribeTagsPaginator,
+        DescribeWarmPoolPaginator,
     )
 
     session = get_session()
     with session.create_client("autoscaling") as client:
         client: AutoScalingClient
 
         describe_auto_scaling_groups_paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator("describe_auto_scaling_groups")
@@ -32,28 +33,30 @@
         describe_load_balancer_target_groups_paginator: DescribeLoadBalancerTargetGroupsPaginator = client.get_paginator("describe_load_balancer_target_groups")
         describe_load_balancers_paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
         describe_notification_configurations_paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")
         describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
         describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
         describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
         describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+        describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
     ```
 """
 from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ActivitiesTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeWarmPoolAnswerTypeDef,
     FilterTypeDef,
     LaunchConfigurationsTypeTypeDef,
     PaginatorConfigTypeDef,
     PoliciesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     TagsTypeTypeDef,
     TimestampTypeDef,
@@ -66,14 +69,15 @@
     "DescribeLoadBalancerTargetGroupsPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeNotificationConfigurationsPaginator",
     "DescribePoliciesPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScheduledActionsPaginator",
     "DescribeTagsPaginator",
+    "DescribeWarmPoolPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -256,7 +260,22 @@
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[TagsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describetagspaginator)
         """
+
+
+class DescribeWarmPoolPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeWarmPool)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describewarmpoolpaginator)
+    """
+
+    def paginate(
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[DescribeWarmPoolAnswerTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeWarmPool.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describewarmpoolpaginator)
+        """
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/paginator.pyi` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         DescribeLoadBalancerTargetGroupsPaginator,
         DescribeLoadBalancersPaginator,
         DescribeNotificationConfigurationsPaginator,
         DescribePoliciesPaginator,
         DescribeScalingActivitiesPaginator,
         DescribeScheduledActionsPaginator,
         DescribeTagsPaginator,
+        DescribeWarmPoolPaginator,
     )
 
     session = get_session()
     with session.create_client("autoscaling") as client:
         client: AutoScalingClient
 
         describe_auto_scaling_groups_paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator("describe_auto_scaling_groups")
@@ -32,28 +33,30 @@
         describe_load_balancer_target_groups_paginator: DescribeLoadBalancerTargetGroupsPaginator = client.get_paginator("describe_load_balancer_target_groups")
         describe_load_balancers_paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
         describe_notification_configurations_paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")
         describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
         describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
         describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
         describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+        describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")
     ```
 """
 from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ActivitiesTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeWarmPoolAnswerTypeDef,
     FilterTypeDef,
     LaunchConfigurationsTypeTypeDef,
     PaginatorConfigTypeDef,
     PoliciesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     TagsTypeTypeDef,
     TimestampTypeDef,
@@ -66,14 +69,15 @@
     "DescribeLoadBalancerTargetGroupsPaginator",
     "DescribeLoadBalancersPaginator",
     "DescribeNotificationConfigurationsPaginator",
     "DescribePoliciesPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScheduledActionsPaginator",
     "DescribeTagsPaginator",
+    "DescribeWarmPoolPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
@@ -244,7 +248,21 @@
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[TagsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describetagspaginator)
         """
+
+class DescribeWarmPoolPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeWarmPool)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describewarmpoolpaginator)
+    """
+
+    def paginate(
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[DescribeWarmPoolAnswerTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeWarmPool.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describewarmpoolpaginator)
+        """
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/type_defs.py` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 __all__ = (
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
     "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
+    "AlarmSpecificationTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
@@ -111,15 +112,14 @@
     "DisableMetricsCollectionQueryRequestTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
-    "RefreshPreferencesTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyTypeDef",
@@ -152,27 +152,29 @@
     "DetachInstancesAnswerTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnterStandbyAnswerTypeDef",
     "ExitStandbyAnswerTypeDef",
     "RollbackInstanceRefreshAnswerTypeDef",
     "StartInstanceRefreshAnswerTypeDef",
     "DescribeAdjustmentTypesAnswerTypeDef",
+    "RefreshPreferencesTypeDef",
     "PolicyARNTypeTypeDef",
     "AttachTrafficSourcesTypeRequestTypeDef",
     "DetachTrafficSourcesTypeRequestTypeDef",
     "AutoScalingGroupNamesTypeRequestTypeDef",
     "DescribeTagsTypeRequestTypeDef",
     "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
     "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
     "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
+    "DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BlockDeviceMappingTypeDef",
@@ -294,14 +296,22 @@
     "AdjustmentTypeTypeDef",
     {
         "AdjustmentType": str,
     },
     total=False,
 )
 
+AlarmSpecificationTypeDef = TypedDict(
+    "AlarmSpecificationTypeDef",
+    {
+        "Alarms": List[str],
+    },
+    total=False,
+)
+
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "AlarmName": str,
         "AlarmARN": str,
     },
     total=False,
@@ -1098,29 +1108,14 @@
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
 )
 
-RefreshPreferencesTypeDef = TypedDict(
-    "RefreshPreferencesTypeDef",
-    {
-        "MinHealthyPercentage": int,
-        "InstanceWarmup": int,
-        "CheckpointPercentages": List[int],
-        "CheckpointDelay": int,
-        "SkipMatching": bool,
-        "AutoRollback": bool,
-        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
-        "StandbyInstances": StandbyInstancesType,
-    },
-    total=False,
-)
-
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
@@ -1404,15 +1399,14 @@
 
 
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
-    total=False,
 )
 
 _RequiredScalingProcessQueryRequestTypeDef = TypedDict(
     "_RequiredScalingProcessQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
@@ -1622,14 +1616,30 @@
     "DescribeAdjustmentTypesAnswerTypeDef",
     {
         "AdjustmentTypes": List[AdjustmentTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RefreshPreferencesTypeDef = TypedDict(
+    "RefreshPreferencesTypeDef",
+    {
+        "MinHealthyPercentage": int,
+        "InstanceWarmup": int,
+        "CheckpointPercentages": List[int],
+        "CheckpointDelay": int,
+        "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
+        "AlarmSpecification": AlarmSpecificationTypeDef,
+    },
+    total=False,
+)
+
 PolicyARNTypeTypeDef = TypedDict(
     "PolicyARNTypeTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1771,14 +1781,36 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef = TypedDict(
+    "_RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef = TypedDict(
+    "_OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef(
+    _RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
+    _OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
+):
+    pass
+
+
 LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     {
         "LaunchConfigurationNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling/type_defs.pyi` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
 __all__ = (
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
     "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
+    "AlarmSpecificationTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
     "PaginatorConfigTypeDef",
@@ -110,15 +111,14 @@
     "DisableMetricsCollectionQueryRequestTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
-    "RefreshPreferencesTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyTypeDef",
@@ -151,27 +151,29 @@
     "DetachInstancesAnswerTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnterStandbyAnswerTypeDef",
     "ExitStandbyAnswerTypeDef",
     "RollbackInstanceRefreshAnswerTypeDef",
     "StartInstanceRefreshAnswerTypeDef",
     "DescribeAdjustmentTypesAnswerTypeDef",
+    "RefreshPreferencesTypeDef",
     "PolicyARNTypeTypeDef",
     "AttachTrafficSourcesTypeRequestTypeDef",
     "DetachTrafficSourcesTypeRequestTypeDef",
     "AutoScalingGroupNamesTypeRequestTypeDef",
     "DescribeTagsTypeRequestTypeDef",
     "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
     "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
     "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
+    "DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BlockDeviceMappingTypeDef",
@@ -291,14 +293,22 @@
     "AdjustmentTypeTypeDef",
     {
         "AdjustmentType": str,
     },
     total=False,
 )
 
+AlarmSpecificationTypeDef = TypedDict(
+    "AlarmSpecificationTypeDef",
+    {
+        "Alarms": List[str],
+    },
+    total=False,
+)
+
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "AlarmName": str,
         "AlarmARN": str,
     },
     total=False,
@@ -1053,29 +1063,14 @@
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
 )
 
-RefreshPreferencesTypeDef = TypedDict(
-    "RefreshPreferencesTypeDef",
-    {
-        "MinHealthyPercentage": int,
-        "InstanceWarmup": int,
-        "CheckpointPercentages": List[int],
-        "CheckpointDelay": int,
-        "SkipMatching": bool,
-        "AutoRollback": bool,
-        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
-        "StandbyInstances": StandbyInstancesType,
-    },
-    total=False,
-)
-
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
@@ -1341,15 +1336,14 @@
     pass
 
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
-    total=False,
 )
 
 _RequiredScalingProcessQueryRequestTypeDef = TypedDict(
     "_RequiredScalingProcessQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
@@ -1553,14 +1547,30 @@
     "DescribeAdjustmentTypesAnswerTypeDef",
     {
         "AdjustmentTypes": List[AdjustmentTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RefreshPreferencesTypeDef = TypedDict(
+    "RefreshPreferencesTypeDef",
+    {
+        "MinHealthyPercentage": int,
+        "InstanceWarmup": int,
+        "CheckpointPercentages": List[int],
+        "CheckpointDelay": int,
+        "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
+        "AlarmSpecification": AlarmSpecificationTypeDef,
+    },
+    total=False,
+)
+
 PolicyARNTypeTypeDef = TypedDict(
     "PolicyARNTypeTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1698,14 +1708,34 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef = TypedDict(
+    "_RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef = TypedDict(
+    "_OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef(
+    _RequiredDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
+    _OptionalDescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef,
+):
+    pass
+
 LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
     "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     {
         "LaunchConfigurationNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling.egg-info/PKG-INFO` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AutoScaling 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AutoScaling 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling)](https://pepy.tech/project/types-aiobotocore-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[aiobotocore.AutoScaling 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -282,14 +282,15 @@
     DescribeLoadBalancerTargetGroupsPaginator,
     DescribeLoadBalancersPaginator,
     DescribeNotificationConfigurationsPaginator,
     DescribePoliciesPaginator,
     DescribeScalingActivitiesPaginator,
     DescribeScheduledActionsPaginator,
     DescribeTagsPaginator,
+    DescribeWarmPoolPaginator,
 )
 
 session = get_session()
 async with session.create_client("autoscaling") as client:
     client: AutoScalingClient
 
     # Explicit type annotations are optional here
@@ -318,14 +319,17 @@
     describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = (
         client.get_paginator("describe_scaling_activities")
     )
     describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator(
         "describe_scheduled_actions"
     )
     describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
+    describe_warm_pool_paginator: DescribeWarmPoolPaginator = client.get_paginator(
+        "describe_warm_pool"
+    )
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_autoscaling.literals` module contains literals extracted
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post3/types_aiobotocore_autoscaling.egg-info/SOURCES.txt` & `types-aiobotocore-autoscaling-2.5.4/types_aiobotocore_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

