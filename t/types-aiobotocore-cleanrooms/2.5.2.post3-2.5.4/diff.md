# Comparing `tmp/types-aiobotocore-cleanrooms-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-cleanrooms-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cleanrooms-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-cleanrooms-2.5.4.tar", last modified: Tue Aug  8 01:23:24 2023, max compression
```

## Comparing `types-aiobotocore-cleanrooms-2.5.2.post3.tar` & `types-aiobotocore-cleanrooms-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.027335 types-aiobotocore-cleanrooms-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-08-04 12:37:24.027335 types-aiobotocore-cleanrooms-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12575 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:24.027335 types-aiobotocore-cleanrooms-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.019335 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31966 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31913 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41235 2023-08-04 12:19:27.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41182 2023-08-04 12:19:27.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:19:26.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:24.027335 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-08-04 12:37:23.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:37:23.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:23.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:23.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:23.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:37:23.000000 types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.630624 types-aiobotocore-cleanrooms-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-08-08 01:23:24.630624 types-aiobotocore-cleanrooms-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:24.630624 types-aiobotocore-cleanrooms-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-08 01:07:09.000000 types-aiobotocore-cleanrooms-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.630624 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38457 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38394 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54222 2023-08-08 01:07:11.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54143 2023-08-08 01:07:11.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:07:10.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:24.630624 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-08-08 01:23:24.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 01:23:24.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:24.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:24.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:24.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 01:23:24.000000 types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/LICENSE` & `types-aiobotocore-cleanrooms-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/PKG-INFO` & `types-aiobotocore-cleanrooms-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cleanrooms
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CleanRoomsService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CleanRoomsService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanrooms)](https://pepy.tech/project/types-aiobotocore-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CleanRoomsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[aiobotocore.CleanRoomsService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -272,14 +272,16 @@
 all paginators.
 
 ```python
 from aiobotocore.session import get_session
 
 from types_aiobotocore_cleanrooms import CleanRoomsServiceClient
 from types_aiobotocore_cleanrooms.paginator import (
+    ListAnalysisTemplatesPaginator,
+    ListCollaborationAnalysisTemplatesPaginator,
     ListCollaborationsPaginator,
     ListConfiguredTableAssociationsPaginator,
     ListConfiguredTablesPaginator,
     ListMembersPaginator,
     ListMembershipsPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
@@ -287,14 +289,20 @@
 
 session = get_session()
 async with session.create_client("cleanrooms") as client:
     client: CleanRoomsServiceClient
 
     # Explicit type annotations are optional here
     # Types should be correctly discovered by mypy and IDEs
+    list_analysis_templates_paginator: ListAnalysisTemplatesPaginator = client.get_paginator(
+        "list_analysis_templates"
+    )
+    list_collaboration_analysis_templates_paginator: ListCollaborationAnalysisTemplatesPaginator = (
+        client.get_paginator("list_collaboration_analysis_templates")
+    )
     list_collaborations_paginator: ListCollaborationsPaginator = client.get_paginator(
         "list_collaborations"
     )
     list_configured_table_associations_paginator: ListConfiguredTableAssociationsPaginator = (
         client.get_paginator("list_configured_table_associations")
     )
     list_configured_tables_paginator: ListConfiguredTablesPaginator = client.get_paginator(
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/README.md` & `types-aiobotocore-cleanrooms-2.5.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanrooms)](https://pepy.tech/project/types-aiobotocore-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CleanRoomsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[aiobotocore.CleanRoomsService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -240,14 +240,16 @@
 all paginators.
 
 ```python
 from aiobotocore.session import get_session
 
 from types_aiobotocore_cleanrooms import CleanRoomsServiceClient
 from types_aiobotocore_cleanrooms.paginator import (
+    ListAnalysisTemplatesPaginator,
+    ListCollaborationAnalysisTemplatesPaginator,
     ListCollaborationsPaginator,
     ListConfiguredTableAssociationsPaginator,
     ListConfiguredTablesPaginator,
     ListMembersPaginator,
     ListMembershipsPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
@@ -255,14 +257,20 @@
 
 session = get_session()
 async with session.create_client("cleanrooms") as client:
     client: CleanRoomsServiceClient
 
     # Explicit type annotations are optional here
     # Types should be correctly discovered by mypy and IDEs
+    list_analysis_templates_paginator: ListAnalysisTemplatesPaginator = client.get_paginator(
+        "list_analysis_templates"
+    )
+    list_collaboration_analysis_templates_paginator: ListCollaborationAnalysisTemplatesPaginator = (
+        client.get_paginator("list_collaboration_analysis_templates")
+    )
     list_collaborations_paginator: ListCollaborationsPaginator = client.get_paginator(
         "list_collaborations"
     )
     list_configured_table_associations_paginator: ListConfiguredTableAssociationsPaginator = (
         client.get_paginator("list_configured_table_associations")
     )
     list_configured_tables_paginator: ListConfiguredTablesPaginator = client.get_paginator(
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/setup.py` & `types-aiobotocore-cleanrooms-2.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cleanrooms",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_cleanrooms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CleanRoomsService 2.5.2 service generated with"
+        "Type annotations for aiobotocore.CleanRoomsService 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/__init__.py` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 Usage::
 
     ```python
     from aiobotocore.session import get_session
     from types_aiobotocore_cleanrooms import (
         CleanRoomsServiceClient,
         Client,
+        ListAnalysisTemplatesPaginator,
+        ListCollaborationAnalysisTemplatesPaginator,
         ListCollaborationsPaginator,
         ListConfiguredTableAssociationsPaginator,
         ListConfiguredTablesPaginator,
         ListMembersPaginator,
         ListMembershipsPaginator,
         ListProtectedQueriesPaginator,
         ListSchemasPaginator,
@@ -19,25 +21,29 @@
 
     session = get_session()
     async with session.create_client("cleanrooms") as client:
         client: CleanRoomsServiceClient
         ...
 
 
+    list_analysis_templates_paginator: ListAnalysisTemplatesPaginator = client.get_paginator("list_analysis_templates")
+    list_collaboration_analysis_templates_paginator: ListCollaborationAnalysisTemplatesPaginator = client.get_paginator("list_collaboration_analysis_templates")
     list_collaborations_paginator: ListCollaborationsPaginator = client.get_paginator("list_collaborations")
     list_configured_table_associations_paginator: ListConfiguredTableAssociationsPaginator = client.get_paginator("list_configured_table_associations")
     list_configured_tables_paginator: ListConfiguredTablesPaginator = client.get_paginator("list_configured_tables")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_memberships_paginator: ListMembershipsPaginator = client.get_paginator("list_memberships")
     list_protected_queries_paginator: ListProtectedQueriesPaginator = client.get_paginator("list_protected_queries")
     list_schemas_paginator: ListSchemasPaginator = client.get_paginator("list_schemas")
     ```
 """
 from .client import CleanRoomsServiceClient
 from .paginator import (
+    ListAnalysisTemplatesPaginator,
+    ListCollaborationAnalysisTemplatesPaginator,
     ListCollaborationsPaginator,
     ListConfiguredTableAssociationsPaginator,
     ListConfiguredTablesPaginator,
     ListMembershipsPaginator,
     ListMembersPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
@@ -45,14 +51,16 @@
 
 Client = CleanRoomsServiceClient
 
 
 __all__ = (
     "CleanRoomsServiceClient",
     "Client",
+    "ListAnalysisTemplatesPaginator",
+    "ListCollaborationAnalysisTemplatesPaginator",
     "ListCollaborationsPaginator",
     "ListConfiguredTableAssociationsPaginator",
     "ListConfiguredTablesPaginator",
     "ListMembersPaginator",
     "ListMembershipsPaginator",
     "ListProtectedQueriesPaginator",
     "ListSchemasPaginator",
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/__init__.pyi` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/__init__.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 Usage::
 
     ```python
     from aiobotocore.session import get_session
     from types_aiobotocore_cleanrooms import (
         CleanRoomsServiceClient,
         Client,
+        ListAnalysisTemplatesPaginator,
+        ListCollaborationAnalysisTemplatesPaginator,
         ListCollaborationsPaginator,
         ListConfiguredTableAssociationsPaginator,
         ListConfiguredTablesPaginator,
         ListMembersPaginator,
         ListMembershipsPaginator,
         ListProtectedQueriesPaginator,
         ListSchemasPaginator,
@@ -19,39 +21,45 @@
 
     session = get_session()
     async with session.create_client("cleanrooms") as client:
         client: CleanRoomsServiceClient
         ...
 
 
+    list_analysis_templates_paginator: ListAnalysisTemplatesPaginator = client.get_paginator("list_analysis_templates")
+    list_collaboration_analysis_templates_paginator: ListCollaborationAnalysisTemplatesPaginator = client.get_paginator("list_collaboration_analysis_templates")
     list_collaborations_paginator: ListCollaborationsPaginator = client.get_paginator("list_collaborations")
     list_configured_table_associations_paginator: ListConfiguredTableAssociationsPaginator = client.get_paginator("list_configured_table_associations")
     list_configured_tables_paginator: ListConfiguredTablesPaginator = client.get_paginator("list_configured_tables")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_memberships_paginator: ListMembershipsPaginator = client.get_paginator("list_memberships")
     list_protected_queries_paginator: ListProtectedQueriesPaginator = client.get_paginator("list_protected_queries")
     list_schemas_paginator: ListSchemasPaginator = client.get_paginator("list_schemas")
     ```
 """
 from .client import CleanRoomsServiceClient
 from .paginator import (
+    ListAnalysisTemplatesPaginator,
+    ListCollaborationAnalysisTemplatesPaginator,
     ListCollaborationsPaginator,
     ListConfiguredTableAssociationsPaginator,
     ListConfiguredTablesPaginator,
     ListMembershipsPaginator,
     ListMembersPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
 )
 
 Client = CleanRoomsServiceClient
 
 __all__ = (
     "CleanRoomsServiceClient",
     "Client",
+    "ListAnalysisTemplatesPaginator",
+    "ListCollaborationAnalysisTemplatesPaginator",
     "ListCollaborationsPaginator",
     "ListConfiguredTableAssociationsPaginator",
     "ListConfiguredTablesPaginator",
     "ListMembersPaginator",
     "ListMembershipsPaginator",
     "ListProtectedQueriesPaginator",
     "ListSchemasPaginator",
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/client.py` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/client.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -27,88 +27,95 @@
     FilterableMemberStatusType,
     MemberAbilityType,
     MembershipQueryLogStatusType,
     MembershipStatusType,
     ProtectedQueryStatusType,
 )
 from .paginator import (
+    ListAnalysisTemplatesPaginator,
+    ListCollaborationAnalysisTemplatesPaginator,
     ListCollaborationsPaginator,
     ListConfiguredTableAssociationsPaginator,
     ListConfiguredTablesPaginator,
     ListMembershipsPaginator,
     ListMembersPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
 )
 from .type_defs import (
+    AnalysisParameterTypeDef,
+    AnalysisSourceTypeDef,
+    BatchGetCollaborationAnalysisTemplateOutputTypeDef,
     BatchGetSchemaOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
+    CreateAnalysisTemplateOutputTypeDef,
     CreateCollaborationOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     CreateConfiguredTableOutputTypeDef,
     CreateMembershipOutputTypeDef,
     DataEncryptionMetadataTypeDef,
+    GetAnalysisTemplateOutputTypeDef,
+    GetCollaborationAnalysisTemplateOutputTypeDef,
     GetCollaborationOutputTypeDef,
     GetConfiguredTableAnalysisRuleOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableOutputTypeDef,
     GetMembershipOutputTypeDef,
     GetProtectedQueryOutputTypeDef,
     GetSchemaAnalysisRuleOutputTypeDef,
     GetSchemaOutputTypeDef,
+    ListAnalysisTemplatesOutputTypeDef,
+    ListCollaborationAnalysisTemplatesOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListMembersOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     MemberSpecificationTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     StartProtectedQueryOutputTypeDef,
     TableReferenceTypeDef,
+    UpdateAnalysisTemplateOutputTypeDef,
     UpdateCollaborationOutputTypeDef,
     UpdateConfiguredTableAnalysisRuleOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableOutputTypeDef,
     UpdateMembershipOutputTypeDef,
     UpdateProtectedQueryOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CleanRoomsServiceClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class CleanRoomsServiceClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/)
     """
 
     meta: ClientMeta
@@ -117,41 +124,64 @@
     def exceptions(self) -> Exceptions:
         """
         CleanRoomsServiceClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#exceptions)
         """
+    async def batch_get_collaboration_analysis_template(
+        self, *, collaborationIdentifier: str, analysisTemplateArns: Sequence[str]
+    ) -> BatchGetCollaborationAnalysisTemplateOutputTypeDef:
+        """
+        Retrieves multiple analysis templates within a collaboration by their Amazon
+        Resource Names (ARNs).
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.batch_get_collaboration_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#batch_get_collaboration_analysis_template)
+        """
     async def batch_get_schema(
         self, *, collaborationIdentifier: str, names: Sequence[str]
     ) -> BatchGetSchemaOutputTypeDef:
         """
         Retrieves multiple schemas by their identifiers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.batch_get_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#batch_get_schema)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#close)
         """
+    async def create_analysis_template(
+        self,
+        *,
+        membershipIdentifier: str,
+        name: str,
+        format: Literal["SQL"],
+        source: AnalysisSourceTypeDef,
+        description: str = ...,
+        tags: Mapping[str, str] = ...,
+        analysisParameters: Sequence[AnalysisParameterTypeDef] = ...
+    ) -> CreateAnalysisTemplateOutputTypeDef:
+        """
+        Creates a new analysis template.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_analysis_template)
+        """
     async def create_collaboration(
         self,
         *,
         members: Sequence[MemberSpecificationTypeDef],
         name: str,
         description: str,
         creatorMemberAbilities: Sequence[MemberAbilityType],
@@ -162,15 +192,14 @@
     ) -> CreateCollaborationOutputTypeDef:
         """
         Creates a new collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_collaboration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_collaboration)
         """
-
     async def create_configured_table(
         self,
         *,
         name: str,
         tableReference: TableReferenceTypeDef,
         allowedColumns: Sequence[str],
         analysisMethod: Literal["DIRECT_QUERY"],
@@ -179,29 +208,27 @@
     ) -> CreateConfiguredTableOutputTypeDef:
         """
         Creates a new configured table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table)
         """
-
     async def create_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
         analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
     ) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Creates a new analysis rule for a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_analysis_rule)
         """
-
     async def create_configured_table_association(
         self,
         *,
         name: str,
         membershipIdentifier: str,
         configuredTableIdentifier: str,
         roleArn: str,
@@ -210,442 +237,470 @@
     ) -> CreateConfiguredTableAssociationOutputTypeDef:
         """
         Creates a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_association)
         """
-
     async def create_membership(
         self,
         *,
         collaborationIdentifier: str,
         queryLogStatus: MembershipQueryLogStatusType,
         tags: Mapping[str, str] = ...
     ) -> CreateMembershipOutputTypeDef:
         """
         Creates a membership for a specific collaboration identifier and joins the
         collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_membership)
         """
+    async def delete_analysis_template(
+        self, *, membershipIdentifier: str, analysisTemplateIdentifier: str
+    ) -> Dict[str, Any]:
+        """
+        Deletes an analysis template.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_analysis_template)
+        """
     async def delete_collaboration(self, *, collaborationIdentifier: str) -> Dict[str, Any]:
         """
         Deletes a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_collaboration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_collaboration)
         """
-
     async def delete_configured_table(self, *, configuredTableIdentifier: str) -> Dict[str, Any]:
         """
         Deletes a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_configured_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_configured_table)
         """
-
     async def delete_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType
     ) -> Dict[str, Any]:
         """
         Deletes a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_configured_table_analysis_rule)
         """
-
     async def delete_configured_table_association(
         self, *, configuredTableAssociationIdentifier: str, membershipIdentifier: str
     ) -> Dict[str, Any]:
         """
         Deletes a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_configured_table_association)
         """
-
     async def delete_member(
         self, *, collaborationIdentifier: str, accountId: str
     ) -> Dict[str, Any]:
         """
         Removes the specified member from a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_member)
         """
-
     async def delete_membership(self, *, membershipIdentifier: str) -> Dict[str, Any]:
         """
         Deletes a specified membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_membership)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#generate_presigned_url)
         """
+    async def get_analysis_template(
+        self, *, membershipIdentifier: str, analysisTemplateIdentifier: str
+    ) -> GetAnalysisTemplateOutputTypeDef:
+        """
+        Retrieves an analysis template.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_analysis_template)
+        """
     async def get_collaboration(
         self, *, collaborationIdentifier: str
     ) -> GetCollaborationOutputTypeDef:
         """
         Returns metadata about a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_collaboration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_collaboration)
         """
+    async def get_collaboration_analysis_template(
+        self, *, collaborationIdentifier: str, analysisTemplateArn: str
+    ) -> GetCollaborationAnalysisTemplateOutputTypeDef:
+        """
+        Retrieves an analysis template within a collaboration.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_collaboration_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_collaboration_analysis_template)
+        """
     async def get_configured_table(
         self, *, configuredTableIdentifier: str
     ) -> GetConfiguredTableOutputTypeDef:
         """
         Retrieves a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_configured_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_configured_table)
         """
-
     async def get_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType
     ) -> GetConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Retrieves a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_configured_table_analysis_rule)
         """
-
     async def get_configured_table_association(
         self, *, configuredTableAssociationIdentifier: str, membershipIdentifier: str
     ) -> GetConfiguredTableAssociationOutputTypeDef:
         """
         Retrieves a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_configured_table_association)
         """
-
     async def get_membership(self, *, membershipIdentifier: str) -> GetMembershipOutputTypeDef:
         """
         Retrieves a specified membership for an identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_membership)
         """
-
     async def get_protected_query(
         self, *, membershipIdentifier: str, protectedQueryIdentifier: str
     ) -> GetProtectedQueryOutputTypeDef:
         """
         Returns query processing metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_protected_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_protected_query)
         """
-
     async def get_schema(
         self, *, collaborationIdentifier: str, name: str
     ) -> GetSchemaOutputTypeDef:
         """
         Retrieves the schema for a relation within a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_schema)
         """
-
     async def get_schema_analysis_rule(
         self, *, collaborationIdentifier: str, name: str, type: AnalysisRuleTypeType
     ) -> GetSchemaAnalysisRuleOutputTypeDef:
         """
         Retrieves a schema analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_schema_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_schema_analysis_rule)
         """
+    async def list_analysis_templates(
+        self, *, membershipIdentifier: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListAnalysisTemplatesOutputTypeDef:
+        """
+        Lists analysis templates that the caller owns.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_analysis_templates)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_analysis_templates)
+        """
+    async def list_collaboration_analysis_templates(
+        self, *, collaborationIdentifier: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListCollaborationAnalysisTemplatesOutputTypeDef:
+        """
+        Lists analysis templates within a collaboration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_collaboration_analysis_templates)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_collaboration_analysis_templates)
+        """
     async def list_collaborations(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         memberStatus: FilterableMemberStatusType = ...
     ) -> ListCollaborationsOutputTypeDef:
         """
         Lists collaborations the caller owns, is active in, or has been invited to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_collaborations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_collaborations)
         """
-
     async def list_configured_table_associations(
         self, *, membershipIdentifier: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListConfiguredTableAssociationsOutputTypeDef:
         """
         Lists configured table associations for a membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_configured_table_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_configured_table_associations)
         """
-
     async def list_configured_tables(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListConfiguredTablesOutputTypeDef:
         """
         Lists configured tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_configured_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_configured_tables)
         """
-
     async def list_members(
         self, *, collaborationIdentifier: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListMembersOutputTypeDef:
         """
         Lists all members within a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_members)
         """
-
     async def list_memberships(
         self, *, nextToken: str = ..., maxResults: int = ..., status: MembershipStatusType = ...
     ) -> ListMembershipsOutputTypeDef:
         """
         Lists all memberships resources within the caller's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_memberships)
         """
-
     async def list_protected_queries(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListProtectedQueriesOutputTypeDef:
         """
         Lists protected queries, sorted by the most recent query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_protected_queries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_protected_queries)
         """
-
     async def list_schemas(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListSchemasOutputTypeDef:
         """
         Lists the schemas for relations within a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_schemas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_schemas)
         """
-
     async def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceOutputTypeDef:
         """
         Lists all of the tags that have been added to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_tags_for_resource)
         """
-
     async def start_protected_query(
         self,
         *,
         type: Literal["SQL"],
         membershipIdentifier: str,
         sqlParameters: ProtectedQuerySQLParametersTypeDef,
         resultConfiguration: ProtectedQueryResultConfigurationTypeDef
     ) -> StartProtectedQueryOutputTypeDef:
         """
-        Creates a protected query that is started by AWS Clean Rooms.
+        Creates a protected query that is started by Clean Rooms .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.start_protected_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#start_protected_query)
         """
-
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Tags a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#tag_resource)
         """
-
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag or list of tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#untag_resource)
         """
+    async def update_analysis_template(
+        self, *, membershipIdentifier: str, analysisTemplateIdentifier: str, description: str = ...
+    ) -> UpdateAnalysisTemplateOutputTypeDef:
+        """
+        Updates the analysis template metadata.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_analysis_template)
+        """
     async def update_collaboration(
         self, *, collaborationIdentifier: str, name: str = ..., description: str = ...
     ) -> UpdateCollaborationOutputTypeDef:
         """
         Updates collaboration metadata and can only be called by the collaboration
         owner.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_collaboration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_collaboration)
         """
-
     async def update_configured_table(
         self, *, configuredTableIdentifier: str, name: str = ..., description: str = ...
     ) -> UpdateConfiguredTableOutputTypeDef:
         """
         Updates a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table)
         """
-
     async def update_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
         analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
     ) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Updates a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_analysis_rule)
         """
-
     async def update_configured_table_association(
         self,
         *,
         configuredTableAssociationIdentifier: str,
         membershipIdentifier: str,
         description: str = ...,
         roleArn: str = ...
     ) -> UpdateConfiguredTableAssociationOutputTypeDef:
         """
         Updates a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_association)
         """
-
     async def update_membership(
         self, *, membershipIdentifier: str, queryLogStatus: MembershipQueryLogStatusType = ...
     ) -> UpdateMembershipOutputTypeDef:
         """
         Updates a membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_membership)
         """
-
     async def update_protected_query(
         self,
         *,
         membershipIdentifier: str,
         protectedQueryIdentifier: str,
         targetStatus: Literal["CANCELLED"]
     ) -> UpdateProtectedQueryOutputTypeDef:
         """
         Updates the processing of a currently running query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_protected_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_protected_query)
         """
-
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_analysis_templates"]
+    ) -> ListAnalysisTemplatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_collaboration_analysis_templates"]
+    ) -> ListCollaborationAnalysisTemplatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
+        """
     @overload
     def get_paginator(
         self, operation_name: Literal["list_collaborations"]
     ) -> ListCollaborationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_configured_table_associations"]
     ) -> ListConfiguredTableAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_configured_tables"]
     ) -> ListConfiguredTablesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_members"]) -> ListMembersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_memberships"]
     ) -> ListMembershipsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_protected_queries"]
     ) -> ListProtectedQueriesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_schemas"]) -> ListSchemasPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "CleanRoomsServiceClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/client.pyi` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,84 +27,99 @@
     FilterableMemberStatusType,
     MemberAbilityType,
     MembershipQueryLogStatusType,
     MembershipStatusType,
     ProtectedQueryStatusType,
 )
 from .paginator import (
+    ListAnalysisTemplatesPaginator,
+    ListCollaborationAnalysisTemplatesPaginator,
     ListCollaborationsPaginator,
     ListConfiguredTableAssociationsPaginator,
     ListConfiguredTablesPaginator,
     ListMembershipsPaginator,
     ListMembersPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
 )
 from .type_defs import (
+    AnalysisParameterTypeDef,
+    AnalysisSourceTypeDef,
+    BatchGetCollaborationAnalysisTemplateOutputTypeDef,
     BatchGetSchemaOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
+    CreateAnalysisTemplateOutputTypeDef,
     CreateCollaborationOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     CreateConfiguredTableOutputTypeDef,
     CreateMembershipOutputTypeDef,
     DataEncryptionMetadataTypeDef,
+    GetAnalysisTemplateOutputTypeDef,
+    GetCollaborationAnalysisTemplateOutputTypeDef,
     GetCollaborationOutputTypeDef,
     GetConfiguredTableAnalysisRuleOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableOutputTypeDef,
     GetMembershipOutputTypeDef,
     GetProtectedQueryOutputTypeDef,
     GetSchemaAnalysisRuleOutputTypeDef,
     GetSchemaOutputTypeDef,
+    ListAnalysisTemplatesOutputTypeDef,
+    ListCollaborationAnalysisTemplatesOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListMembersOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     MemberSpecificationTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     StartProtectedQueryOutputTypeDef,
     TableReferenceTypeDef,
+    UpdateAnalysisTemplateOutputTypeDef,
     UpdateCollaborationOutputTypeDef,
     UpdateConfiguredTableAnalysisRuleOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableOutputTypeDef,
     UpdateMembershipOutputTypeDef,
     UpdateProtectedQueryOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("CleanRoomsServiceClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class CleanRoomsServiceClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/)
     """
 
     meta: ClientMeta
@@ -113,37 +128,70 @@
     def exceptions(self) -> Exceptions:
         """
         CleanRoomsServiceClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#exceptions)
         """
+
+    async def batch_get_collaboration_analysis_template(
+        self, *, collaborationIdentifier: str, analysisTemplateArns: Sequence[str]
+    ) -> BatchGetCollaborationAnalysisTemplateOutputTypeDef:
+        """
+        Retrieves multiple analysis templates within a collaboration by their Amazon
+        Resource Names (ARNs).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.batch_get_collaboration_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#batch_get_collaboration_analysis_template)
+        """
+
     async def batch_get_schema(
         self, *, collaborationIdentifier: str, names: Sequence[str]
     ) -> BatchGetSchemaOutputTypeDef:
         """
         Retrieves multiple schemas by their identifiers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.batch_get_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#batch_get_schema)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#close)
         """
+
+    async def create_analysis_template(
+        self,
+        *,
+        membershipIdentifier: str,
+        name: str,
+        format: Literal["SQL"],
+        source: AnalysisSourceTypeDef,
+        description: str = ...,
+        tags: Mapping[str, str] = ...,
+        analysisParameters: Sequence[AnalysisParameterTypeDef] = ...
+    ) -> CreateAnalysisTemplateOutputTypeDef:
+        """
+        Creates a new analysis template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_analysis_template)
+        """
+
     async def create_collaboration(
         self,
         *,
         members: Sequence[MemberSpecificationTypeDef],
         name: str,
         description: str,
         creatorMemberAbilities: Sequence[MemberAbilityType],
@@ -154,14 +202,15 @@
     ) -> CreateCollaborationOutputTypeDef:
         """
         Creates a new collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_collaboration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_collaboration)
         """
+
     async def create_configured_table(
         self,
         *,
         name: str,
         tableReference: TableReferenceTypeDef,
         allowedColumns: Sequence[str],
         analysisMethod: Literal["DIRECT_QUERY"],
@@ -170,27 +219,29 @@
     ) -> CreateConfiguredTableOutputTypeDef:
         """
         Creates a new configured table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table)
         """
+
     async def create_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
         analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
     ) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Creates a new analysis rule for a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_analysis_rule)
         """
+
     async def create_configured_table_association(
         self,
         *,
         name: str,
         membershipIdentifier: str,
         configuredTableIdentifier: str,
         roleArn: str,
@@ -199,400 +250,520 @@
     ) -> CreateConfiguredTableAssociationOutputTypeDef:
         """
         Creates a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_association)
         """
+
     async def create_membership(
         self,
         *,
         collaborationIdentifier: str,
         queryLogStatus: MembershipQueryLogStatusType,
         tags: Mapping[str, str] = ...
     ) -> CreateMembershipOutputTypeDef:
         """
         Creates a membership for a specific collaboration identifier and joins the
         collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_membership)
         """
+
+    async def delete_analysis_template(
+        self, *, membershipIdentifier: str, analysisTemplateIdentifier: str
+    ) -> Dict[str, Any]:
+        """
+        Deletes an analysis template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_analysis_template)
+        """
+
     async def delete_collaboration(self, *, collaborationIdentifier: str) -> Dict[str, Any]:
         """
         Deletes a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_collaboration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_collaboration)
         """
+
     async def delete_configured_table(self, *, configuredTableIdentifier: str) -> Dict[str, Any]:
         """
         Deletes a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_configured_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_configured_table)
         """
+
     async def delete_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType
     ) -> Dict[str, Any]:
         """
         Deletes a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_configured_table_analysis_rule)
         """
+
     async def delete_configured_table_association(
         self, *, configuredTableAssociationIdentifier: str, membershipIdentifier: str
     ) -> Dict[str, Any]:
         """
         Deletes a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_configured_table_association)
         """
+
     async def delete_member(
         self, *, collaborationIdentifier: str, accountId: str
     ) -> Dict[str, Any]:
         """
         Removes the specified member from a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_member)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_member)
         """
+
     async def delete_membership(self, *, membershipIdentifier: str) -> Dict[str, Any]:
         """
         Deletes a specified membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_membership)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#generate_presigned_url)
         """
+
+    async def get_analysis_template(
+        self, *, membershipIdentifier: str, analysisTemplateIdentifier: str
+    ) -> GetAnalysisTemplateOutputTypeDef:
+        """
+        Retrieves an analysis template.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_analysis_template)
+        """
+
     async def get_collaboration(
         self, *, collaborationIdentifier: str
     ) -> GetCollaborationOutputTypeDef:
         """
         Returns metadata about a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_collaboration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_collaboration)
         """
+
+    async def get_collaboration_analysis_template(
+        self, *, collaborationIdentifier: str, analysisTemplateArn: str
+    ) -> GetCollaborationAnalysisTemplateOutputTypeDef:
+        """
+        Retrieves an analysis template within a collaboration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_collaboration_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_collaboration_analysis_template)
+        """
+
     async def get_configured_table(
         self, *, configuredTableIdentifier: str
     ) -> GetConfiguredTableOutputTypeDef:
         """
         Retrieves a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_configured_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_configured_table)
         """
+
     async def get_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType
     ) -> GetConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Retrieves a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_configured_table_analysis_rule)
         """
+
     async def get_configured_table_association(
         self, *, configuredTableAssociationIdentifier: str, membershipIdentifier: str
     ) -> GetConfiguredTableAssociationOutputTypeDef:
         """
         Retrieves a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_configured_table_association)
         """
+
     async def get_membership(self, *, membershipIdentifier: str) -> GetMembershipOutputTypeDef:
         """
         Retrieves a specified membership for an identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_membership)
         """
+
     async def get_protected_query(
         self, *, membershipIdentifier: str, protectedQueryIdentifier: str
     ) -> GetProtectedQueryOutputTypeDef:
         """
         Returns query processing metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_protected_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_protected_query)
         """
+
     async def get_schema(
         self, *, collaborationIdentifier: str, name: str
     ) -> GetSchemaOutputTypeDef:
         """
         Retrieves the schema for a relation within a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_schema)
         """
+
     async def get_schema_analysis_rule(
         self, *, collaborationIdentifier: str, name: str, type: AnalysisRuleTypeType
     ) -> GetSchemaAnalysisRuleOutputTypeDef:
         """
         Retrieves a schema analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_schema_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_schema_analysis_rule)
         """
+
+    async def list_analysis_templates(
+        self, *, membershipIdentifier: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListAnalysisTemplatesOutputTypeDef:
+        """
+        Lists analysis templates that the caller owns.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_analysis_templates)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_analysis_templates)
+        """
+
+    async def list_collaboration_analysis_templates(
+        self, *, collaborationIdentifier: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListCollaborationAnalysisTemplatesOutputTypeDef:
+        """
+        Lists analysis templates within a collaboration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_collaboration_analysis_templates)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_collaboration_analysis_templates)
+        """
+
     async def list_collaborations(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         memberStatus: FilterableMemberStatusType = ...
     ) -> ListCollaborationsOutputTypeDef:
         """
         Lists collaborations the caller owns, is active in, or has been invited to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_collaborations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_collaborations)
         """
+
     async def list_configured_table_associations(
         self, *, membershipIdentifier: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListConfiguredTableAssociationsOutputTypeDef:
         """
         Lists configured table associations for a membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_configured_table_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_configured_table_associations)
         """
+
     async def list_configured_tables(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListConfiguredTablesOutputTypeDef:
         """
         Lists configured tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_configured_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_configured_tables)
         """
+
     async def list_members(
         self, *, collaborationIdentifier: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListMembersOutputTypeDef:
         """
         Lists all members within a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_members)
         """
+
     async def list_memberships(
         self, *, nextToken: str = ..., maxResults: int = ..., status: MembershipStatusType = ...
     ) -> ListMembershipsOutputTypeDef:
         """
         Lists all memberships resources within the caller's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_memberships)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_memberships)
         """
+
     async def list_protected_queries(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListProtectedQueriesOutputTypeDef:
         """
         Lists protected queries, sorted by the most recent query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_protected_queries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_protected_queries)
         """
+
     async def list_schemas(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListSchemasOutputTypeDef:
         """
         Lists the schemas for relations within a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_schemas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_schemas)
         """
+
     async def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceOutputTypeDef:
         """
         Lists all of the tags that have been added to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_tags_for_resource)
         """
+
     async def start_protected_query(
         self,
         *,
         type: Literal["SQL"],
         membershipIdentifier: str,
         sqlParameters: ProtectedQuerySQLParametersTypeDef,
         resultConfiguration: ProtectedQueryResultConfigurationTypeDef
     ) -> StartProtectedQueryOutputTypeDef:
         """
-        Creates a protected query that is started by AWS Clean Rooms.
+        Creates a protected query that is started by Clean Rooms .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.start_protected_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#start_protected_query)
         """
+
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Tags a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#tag_resource)
         """
+
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag or list of tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#untag_resource)
         """
+
+    async def update_analysis_template(
+        self, *, membershipIdentifier: str, analysisTemplateIdentifier: str, description: str = ...
+    ) -> UpdateAnalysisTemplateOutputTypeDef:
+        """
+        Updates the analysis template metadata.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_analysis_template)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_analysis_template)
+        """
+
     async def update_collaboration(
         self, *, collaborationIdentifier: str, name: str = ..., description: str = ...
     ) -> UpdateCollaborationOutputTypeDef:
         """
         Updates collaboration metadata and can only be called by the collaboration
         owner.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_collaboration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_collaboration)
         """
+
     async def update_configured_table(
         self, *, configuredTableIdentifier: str, name: str = ..., description: str = ...
     ) -> UpdateConfiguredTableOutputTypeDef:
         """
         Updates a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table)
         """
+
     async def update_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
         analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
     ) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Updates a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_analysis_rule)
         """
+
     async def update_configured_table_association(
         self,
         *,
         configuredTableAssociationIdentifier: str,
         membershipIdentifier: str,
         description: str = ...,
         roleArn: str = ...
     ) -> UpdateConfiguredTableAssociationOutputTypeDef:
         """
         Updates a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_association)
         """
+
     async def update_membership(
         self, *, membershipIdentifier: str, queryLogStatus: MembershipQueryLogStatusType = ...
     ) -> UpdateMembershipOutputTypeDef:
         """
         Updates a membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_membership)
         """
+
     async def update_protected_query(
         self,
         *,
         membershipIdentifier: str,
         protectedQueryIdentifier: str,
         targetStatus: Literal["CANCELLED"]
     ) -> UpdateProtectedQueryOutputTypeDef:
         """
         Updates the processing of a currently running query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_protected_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_protected_query)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_analysis_templates"]
+    ) -> ListAnalysisTemplatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_collaboration_analysis_templates"]
+    ) -> ListCollaborationAnalysisTemplatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_collaborations"]
     ) -> ListCollaborationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_configured_table_associations"]
     ) -> ListConfiguredTableAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_configured_tables"]
     ) -> ListConfiguredTablesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_members"]) -> ListMembersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_memberships"]
     ) -> ListMembershipsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_protected_queries"]
     ) -> ListProtectedQueriesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_schemas"]) -> ListSchemasPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "CleanRoomsServiceClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/literals.py` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,36 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AggregateFunctionNameType",
     "AggregationTypeType",
+    "AnalysisFormatType",
     "AnalysisMethodType",
     "AnalysisRuleTypeType",
     "CollaborationQueryLogStatusType",
     "ConfiguredTableAnalysisRuleTypeType",
     "FilterableMemberStatusType",
+    "JoinOperatorType",
     "JoinRequiredOptionType",
+    "ListAnalysisTemplatesPaginatorName",
+    "ListCollaborationAnalysisTemplatesPaginatorName",
     "ListCollaborationsPaginatorName",
     "ListConfiguredTableAssociationsPaginatorName",
     "ListConfiguredTablesPaginatorName",
     "ListMembersPaginatorName",
     "ListMembershipsPaginatorName",
     "ListProtectedQueriesPaginatorName",
     "ListSchemasPaginatorName",
     "MemberAbilityType",
     "MemberStatusType",
     "MembershipQueryLogStatusType",
     "MembershipStatusType",
+    "ParameterTypeType",
     "ProtectedQueryStatusType",
     "ProtectedQueryTypeType",
     "ResultFormatType",
     "ScalarFunctionsType",
     "SchemaTypeType",
     "TargetProtectedQueryStatusType",
     "CleanRoomsServiceServiceName",
@@ -51,31 +56,52 @@
     "PaginatorName",
     "RegionName",
 )
 
 
 AggregateFunctionNameType = Literal["AVG", "COUNT", "COUNT_DISTINCT", "SUM", "SUM_DISTINCT"]
 AggregationTypeType = Literal["COUNT_DISTINCT"]
+AnalysisFormatType = Literal["SQL"]
 AnalysisMethodType = Literal["DIRECT_QUERY"]
-AnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
+AnalysisRuleTypeType = Literal["AGGREGATION", "CUSTOM", "LIST"]
 CollaborationQueryLogStatusType = Literal["DISABLED", "ENABLED"]
-ConfiguredTableAnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
+ConfiguredTableAnalysisRuleTypeType = Literal["AGGREGATION", "CUSTOM", "LIST"]
 FilterableMemberStatusType = Literal["ACTIVE", "INVITED"]
+JoinOperatorType = Literal["AND", "OR"]
 JoinRequiredOptionType = Literal["QUERY_RUNNER"]
+ListAnalysisTemplatesPaginatorName = Literal["list_analysis_templates"]
+ListCollaborationAnalysisTemplatesPaginatorName = Literal["list_collaboration_analysis_templates"]
 ListCollaborationsPaginatorName = Literal["list_collaborations"]
 ListConfiguredTableAssociationsPaginatorName = Literal["list_configured_table_associations"]
 ListConfiguredTablesPaginatorName = Literal["list_configured_tables"]
 ListMembersPaginatorName = Literal["list_members"]
 ListMembershipsPaginatorName = Literal["list_memberships"]
 ListProtectedQueriesPaginatorName = Literal["list_protected_queries"]
 ListSchemasPaginatorName = Literal["list_schemas"]
 MemberAbilityType = Literal["CAN_QUERY", "CAN_RECEIVE_RESULTS"]
 MemberStatusType = Literal["ACTIVE", "INVITED", "LEFT", "REMOVED"]
 MembershipQueryLogStatusType = Literal["DISABLED", "ENABLED"]
 MembershipStatusType = Literal["ACTIVE", "COLLABORATION_DELETED", "REMOVED"]
+ParameterTypeType = Literal[
+    "BIGINT",
+    "BOOLEAN",
+    "CHAR",
+    "DATE",
+    "DECIMAL",
+    "DOUBLE_PRECISION",
+    "INTEGER",
+    "REAL",
+    "SMALLINT",
+    "TIME",
+    "TIMESTAMP",
+    "TIMESTAMPTZ",
+    "TIMETZ",
+    "VARBYTE",
+    "VARCHAR",
+]
 ProtectedQueryStatusType = Literal[
     "CANCELLED", "CANCELLING", "FAILED", "STARTED", "SUBMITTED", "SUCCESS", "TIMED_OUT"
 ]
 ProtectedQueryTypeType = Literal["SQL"]
 ResultFormatType = Literal["CSV", "PARQUET"]
 ScalarFunctionsType = Literal[
     "ABS",
@@ -106,14 +132,15 @@
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
@@ -209,14 +236,15 @@
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
@@ -295,26 +323,28 @@
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
@@ -455,14 +485,16 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
+    "list_analysis_templates",
+    "list_collaboration_analysis_templates",
     "list_collaborations",
     "list_configured_table_associations",
     "list_configured_tables",
     "list_members",
     "list_memberships",
     "list_protected_queries",
     "list_schemas",
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/literals.pyi` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/literals.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -17,31 +17,36 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AggregateFunctionNameType",
     "AggregationTypeType",
+    "AnalysisFormatType",
     "AnalysisMethodType",
     "AnalysisRuleTypeType",
     "CollaborationQueryLogStatusType",
     "ConfiguredTableAnalysisRuleTypeType",
     "FilterableMemberStatusType",
+    "JoinOperatorType",
     "JoinRequiredOptionType",
+    "ListAnalysisTemplatesPaginatorName",
+    "ListCollaborationAnalysisTemplatesPaginatorName",
     "ListCollaborationsPaginatorName",
     "ListConfiguredTableAssociationsPaginatorName",
     "ListConfiguredTablesPaginatorName",
     "ListMembersPaginatorName",
     "ListMembershipsPaginatorName",
     "ListProtectedQueriesPaginatorName",
     "ListSchemasPaginatorName",
     "MemberAbilityType",
     "MemberStatusType",
     "MembershipQueryLogStatusType",
     "MembershipStatusType",
+    "ParameterTypeType",
     "ProtectedQueryStatusType",
     "ProtectedQueryTypeType",
     "ResultFormatType",
     "ScalarFunctionsType",
     "SchemaTypeType",
     "TargetProtectedQueryStatusType",
     "CleanRoomsServiceServiceName",
@@ -49,31 +54,52 @@
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AggregateFunctionNameType = Literal["AVG", "COUNT", "COUNT_DISTINCT", "SUM", "SUM_DISTINCT"]
 AggregationTypeType = Literal["COUNT_DISTINCT"]
+AnalysisFormatType = Literal["SQL"]
 AnalysisMethodType = Literal["DIRECT_QUERY"]
-AnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
+AnalysisRuleTypeType = Literal["AGGREGATION", "CUSTOM", "LIST"]
 CollaborationQueryLogStatusType = Literal["DISABLED", "ENABLED"]
-ConfiguredTableAnalysisRuleTypeType = Literal["AGGREGATION", "LIST"]
+ConfiguredTableAnalysisRuleTypeType = Literal["AGGREGATION", "CUSTOM", "LIST"]
 FilterableMemberStatusType = Literal["ACTIVE", "INVITED"]
+JoinOperatorType = Literal["AND", "OR"]
 JoinRequiredOptionType = Literal["QUERY_RUNNER"]
+ListAnalysisTemplatesPaginatorName = Literal["list_analysis_templates"]
+ListCollaborationAnalysisTemplatesPaginatorName = Literal["list_collaboration_analysis_templates"]
 ListCollaborationsPaginatorName = Literal["list_collaborations"]
 ListConfiguredTableAssociationsPaginatorName = Literal["list_configured_table_associations"]
 ListConfiguredTablesPaginatorName = Literal["list_configured_tables"]
 ListMembersPaginatorName = Literal["list_members"]
 ListMembershipsPaginatorName = Literal["list_memberships"]
 ListProtectedQueriesPaginatorName = Literal["list_protected_queries"]
 ListSchemasPaginatorName = Literal["list_schemas"]
 MemberAbilityType = Literal["CAN_QUERY", "CAN_RECEIVE_RESULTS"]
 MemberStatusType = Literal["ACTIVE", "INVITED", "LEFT", "REMOVED"]
 MembershipQueryLogStatusType = Literal["DISABLED", "ENABLED"]
 MembershipStatusType = Literal["ACTIVE", "COLLABORATION_DELETED", "REMOVED"]
+ParameterTypeType = Literal[
+    "BIGINT",
+    "BOOLEAN",
+    "CHAR",
+    "DATE",
+    "DECIMAL",
+    "DOUBLE_PRECISION",
+    "INTEGER",
+    "REAL",
+    "SMALLINT",
+    "TIME",
+    "TIMESTAMP",
+    "TIMESTAMPTZ",
+    "TIMETZ",
+    "VARBYTE",
+    "VARCHAR",
+]
 ProtectedQueryStatusType = Literal[
     "CANCELLED", "CANCELLING", "FAILED", "STARTED", "SUBMITTED", "SUCCESS", "TIMED_OUT"
 ]
 ProtectedQueryTypeType = Literal["SQL"]
 ResultFormatType = Literal["CSV", "PARQUET"]
 ScalarFunctionsType = Literal[
     "ABS",
@@ -104,14 +130,15 @@
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
@@ -207,14 +234,15 @@
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
@@ -293,26 +321,28 @@
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
@@ -453,14 +483,16 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
+    "list_analysis_templates",
+    "list_collaboration_analysis_templates",
     "list_collaborations",
     "list_configured_table_associations",
     "list_configured_tables",
     "list_members",
     "list_memberships",
     "list_protected_queries",
     "list_schemas",
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/paginator.py` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/paginator.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -6,27 +6,31 @@
 Usage::
 
     ```python
     from aiobotocore.session import get_session
 
     from types_aiobotocore_cleanrooms.client import CleanRoomsServiceClient
     from types_aiobotocore_cleanrooms.paginator import (
+        ListAnalysisTemplatesPaginator,
+        ListCollaborationAnalysisTemplatesPaginator,
         ListCollaborationsPaginator,
         ListConfiguredTableAssociationsPaginator,
         ListConfiguredTablesPaginator,
         ListMembersPaginator,
         ListMembershipsPaginator,
         ListProtectedQueriesPaginator,
         ListSchemasPaginator,
     )
 
     session = get_session()
     with session.create_client("cleanrooms") as client:
         client: CleanRoomsServiceClient
 
+        list_analysis_templates_paginator: ListAnalysisTemplatesPaginator = client.get_paginator("list_analysis_templates")
+        list_collaboration_analysis_templates_paginator: ListCollaborationAnalysisTemplatesPaginator = client.get_paginator("list_collaboration_analysis_templates")
         list_collaborations_paginator: ListCollaborationsPaginator = client.get_paginator("list_collaborations")
         list_configured_table_associations_paginator: ListConfiguredTableAssociationsPaginator = client.get_paginator("list_configured_table_associations")
         list_configured_tables_paginator: ListConfiguredTablesPaginator = client.get_paginator("list_configured_tables")
         list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
         list_memberships_paginator: ListMembershipsPaginator = client.get_paginator("list_memberships")
         list_protected_queries_paginator: ListProtectedQueriesPaginator = client.get_paginator("list_protected_queries")
         list_schemas_paginator: ListSchemasPaginator = client.get_paginator("list_schemas")
@@ -36,14 +40,16 @@
 from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import FilterableMemberStatusType, MembershipStatusType, ProtectedQueryStatusType
 from .type_defs import (
+    ListAnalysisTemplatesOutputTypeDef,
+    ListCollaborationAnalysisTemplatesOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListMembersOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
@@ -51,35 +57,61 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
+    "ListAnalysisTemplatesPaginator",
+    "ListCollaborationAnalysisTemplatesPaginator",
     "ListCollaborationsPaginator",
     "ListConfiguredTableAssociationsPaginator",
     "ListConfiguredTablesPaginator",
     "ListMembersPaginator",
     "ListMembershipsPaginator",
     "ListProtectedQueriesPaginator",
     "ListSchemasPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+class ListAnalysisTemplatesPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListAnalysisTemplates)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listanalysistemplatespaginator)
+    """
+
+    def paginate(
+        self, *, membershipIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListAnalysisTemplatesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListAnalysisTemplates.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listanalysistemplatespaginator)
+        """
+
+class ListCollaborationAnalysisTemplatesPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborationAnalysisTemplates)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationanalysistemplatespaginator)
+    """
+
+    def paginate(
+        self, *, collaborationIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListCollaborationAnalysisTemplatesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborationAnalysisTemplates.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationanalysistemplatespaginator)
+        """
 
 class ListCollaborationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
     """
 
@@ -90,75 +122,70 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCollaborationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
         """
 
-
 class ListConfiguredTableAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
     """
 
     def paginate(
         self, *, membershipIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfiguredTableAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
         """
 
-
 class ListConfiguredTablesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtablespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfiguredTablesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtablespaginator)
         """
 
-
 class ListMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmemberspaginator)
     """
 
     def paginate(
         self, *, collaborationIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmemberspaginator)
         """
 
-
 class ListMembershipsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmembershipspaginator)
     """
 
     def paginate(
         self, *, status: MembershipStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembershipsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmembershipspaginator)
         """
 
-
 class ListProtectedQueriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listprotectedqueriespaginator)
     """
 
     def paginate(
@@ -169,15 +196,14 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProtectedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listprotectedqueriespaginator)
         """
 
-
 class ListSchemasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listschemaspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/paginator.pyi` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/paginator.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,27 +6,31 @@
 Usage::
 
     ```python
     from aiobotocore.session import get_session
 
     from types_aiobotocore_cleanrooms.client import CleanRoomsServiceClient
     from types_aiobotocore_cleanrooms.paginator import (
+        ListAnalysisTemplatesPaginator,
+        ListCollaborationAnalysisTemplatesPaginator,
         ListCollaborationsPaginator,
         ListConfiguredTableAssociationsPaginator,
         ListConfiguredTablesPaginator,
         ListMembersPaginator,
         ListMembershipsPaginator,
         ListProtectedQueriesPaginator,
         ListSchemasPaginator,
     )
 
     session = get_session()
     with session.create_client("cleanrooms") as client:
         client: CleanRoomsServiceClient
 
+        list_analysis_templates_paginator: ListAnalysisTemplatesPaginator = client.get_paginator("list_analysis_templates")
+        list_collaboration_analysis_templates_paginator: ListCollaborationAnalysisTemplatesPaginator = client.get_paginator("list_collaboration_analysis_templates")
         list_collaborations_paginator: ListCollaborationsPaginator = client.get_paginator("list_collaborations")
         list_configured_table_associations_paginator: ListConfiguredTableAssociationsPaginator = client.get_paginator("list_configured_table_associations")
         list_configured_tables_paginator: ListConfiguredTablesPaginator = client.get_paginator("list_configured_tables")
         list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
         list_memberships_paginator: ListMembershipsPaginator = client.get_paginator("list_memberships")
         list_protected_queries_paginator: ListProtectedQueriesPaginator = client.get_paginator("list_protected_queries")
         list_schemas_paginator: ListSchemasPaginator = client.get_paginator("list_schemas")
@@ -36,14 +40,16 @@
 from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import FilterableMemberStatusType, MembershipStatusType, ProtectedQueryStatusType
 from .type_defs import (
+    ListAnalysisTemplatesOutputTypeDef,
+    ListCollaborationAnalysisTemplatesOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListMembersOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
@@ -51,32 +57,68 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
+    "ListAnalysisTemplatesPaginator",
+    "ListCollaborationAnalysisTemplatesPaginator",
     "ListCollaborationsPaginator",
     "ListConfiguredTableAssociationsPaginator",
     "ListConfiguredTablesPaginator",
     "ListMembersPaginator",
     "ListMembershipsPaginator",
     "ListProtectedQueriesPaginator",
     "ListSchemasPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
+class ListAnalysisTemplatesPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListAnalysisTemplates)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listanalysistemplatespaginator)
+    """
+
+    def paginate(
+        self, *, membershipIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListAnalysisTemplatesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListAnalysisTemplates.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listanalysistemplatespaginator)
+        """
+
+
+class ListCollaborationAnalysisTemplatesPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborationAnalysisTemplates)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationanalysistemplatespaginator)
+    """
+
+    def paginate(
+        self, *, collaborationIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListCollaborationAnalysisTemplatesOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborationAnalysisTemplates.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationanalysistemplatespaginator)
+        """
+
+
 class ListCollaborationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
     """
 
     def paginate(
@@ -86,70 +128,75 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCollaborationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
         """
 
+
 class ListConfiguredTableAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
     """
 
     def paginate(
         self, *, membershipIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfiguredTableAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
         """
 
+
 class ListConfiguredTablesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtablespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfiguredTablesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtablespaginator)
         """
 
+
 class ListMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmemberspaginator)
     """
 
     def paginate(
         self, *, collaborationIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmemberspaginator)
         """
 
+
 class ListMembershipsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmembershipspaginator)
     """
 
     def paginate(
         self, *, status: MembershipStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembershipsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmembershipspaginator)
         """
 
+
 class ListProtectedQueriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listprotectedqueriespaginator)
     """
 
     def paginate(
@@ -160,14 +207,15 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProtectedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listprotectedqueriespaginator)
         """
 
+
 class ListSchemasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listschemaspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/type_defs.py` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/type_defs.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
+    JoinOperatorType,
     MemberAbilityType,
     MembershipQueryLogStatusType,
     MembershipStatusType,
     MemberStatusType,
+    ParameterTypeType,
     ProtectedQueryStatusType,
     ResultFormatType,
     ScalarFunctionsType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -39,44 +41,57 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AggregateColumnTypeDef",
     "AggregationConstraintTypeDef",
+    "AnalysisParameterTypeDef",
+    "AnalysisRuleCustomTypeDef",
     "AnalysisRuleListTypeDef",
+    "AnalysisSchemaTypeDef",
+    "AnalysisSourceTypeDef",
+    "AnalysisTemplateSummaryTypeDef",
+    "BatchGetCollaborationAnalysisTemplateErrorTypeDef",
+    "BatchGetCollaborationAnalysisTemplateInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CollaborationAnalysisTemplateSummaryTypeDef",
     "CollaborationSummaryTypeDef",
     "DataEncryptionMetadataTypeDef",
     "ColumnTypeDef",
     "ConfiguredTableAssociationSummaryTypeDef",
     "ConfiguredTableAssociationTypeDef",
     "ConfiguredTableSummaryTypeDef",
     "MemberSpecificationTypeDef",
     "CreateConfiguredTableAssociationInputRequestTypeDef",
     "CreateMembershipInputRequestTypeDef",
     "MembershipTypeDef",
+    "DeleteAnalysisTemplateInputRequestTypeDef",
     "DeleteCollaborationInputRequestTypeDef",
     "DeleteConfiguredTableAnalysisRuleInputRequestTypeDef",
     "DeleteConfiguredTableAssociationInputRequestTypeDef",
     "DeleteConfiguredTableInputRequestTypeDef",
     "DeleteMemberInputRequestTypeDef",
     "DeleteMembershipInputRequestTypeDef",
+    "GetAnalysisTemplateInputRequestTypeDef",
+    "GetCollaborationAnalysisTemplateInputRequestTypeDef",
     "GetCollaborationInputRequestTypeDef",
     "GetConfiguredTableAnalysisRuleInputRequestTypeDef",
     "GetConfiguredTableAssociationInputRequestTypeDef",
     "GetConfiguredTableInputRequestTypeDef",
     "GetMembershipInputRequestTypeDef",
     "GetProtectedQueryInputRequestTypeDef",
     "GetSchemaAnalysisRuleInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "GlueTableReferenceTypeDef",
     "PaginatorConfigTypeDef",
+    "ListAnalysisTemplatesInputRequestTypeDef",
+    "ListCollaborationAnalysisTemplatesInputRequestTypeDef",
     "ListCollaborationsInputRequestTypeDef",
     "ListConfiguredTableAssociationsInputRequestTypeDef",
     "ListConfiguredTablesInputRequestTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
     "ListMembershipsInputRequestTypeDef",
     "MembershipSummaryTypeDef",
@@ -88,34 +103,42 @@
     "ProtectedQueryErrorTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "UpdateAnalysisTemplateInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
     "AnalysisRuleAggregationTypeDef",
+    "AnalysisTemplateTypeDef",
+    "CollaborationAnalysisTemplateTypeDef",
+    "CreateAnalysisTemplateInputRequestTypeDef",
+    "ListAnalysisTemplatesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "ListCollaborationAnalysisTemplatesOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
     "ListConfiguredTablesOutputTypeDef",
     "CreateCollaborationInputRequestTypeDef",
     "CreateMembershipOutputTypeDef",
     "GetMembershipOutputTypeDef",
     "UpdateMembershipOutputTypeDef",
     "TableReferenceTypeDef",
+    "ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef",
+    "ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef",
     "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
     "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
     "ListMembersInputListMembersPaginateTypeDef",
     "ListMembershipsInputListMembershipsPaginateTypeDef",
     "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
     "ListSchemasInputListSchemasPaginateTypeDef",
@@ -123,14 +146,19 @@
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
+    "CreateAnalysisTemplateOutputTypeDef",
+    "GetAnalysisTemplateOutputTypeDef",
+    "UpdateAnalysisTemplateOutputTypeDef",
+    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
+    "GetCollaborationAnalysisTemplateOutputTypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "BatchGetSchemaOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "ConfiguredTableTypeDef",
     "CreateConfiguredTableInputRequestTypeDef",
@@ -169,50 +197,196 @@
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
 )
 
-AnalysisRuleListTypeDef = TypedDict(
-    "AnalysisRuleListTypeDef",
+_RequiredAnalysisParameterTypeDef = TypedDict(
+    "_RequiredAnalysisParameterTypeDef",
+    {
+        "name": str,
+        "type": ParameterTypeType,
+    },
+)
+_OptionalAnalysisParameterTypeDef = TypedDict(
+    "_OptionalAnalysisParameterTypeDef",
+    {
+        "defaultValue": str,
+    },
+    total=False,
+)
+
+
+class AnalysisParameterTypeDef(
+    _RequiredAnalysisParameterTypeDef, _OptionalAnalysisParameterTypeDef
+):
+    pass
+
+
+_RequiredAnalysisRuleCustomTypeDef = TypedDict(
+    "_RequiredAnalysisRuleCustomTypeDef",
+    {
+        "allowedAnalyses": Sequence[str],
+    },
+)
+_OptionalAnalysisRuleCustomTypeDef = TypedDict(
+    "_OptionalAnalysisRuleCustomTypeDef",
+    {
+        "allowedAnalysisProviders": Sequence[str],
+    },
+    total=False,
+)
+
+
+class AnalysisRuleCustomTypeDef(
+    _RequiredAnalysisRuleCustomTypeDef, _OptionalAnalysisRuleCustomTypeDef
+):
+    pass
+
+
+_RequiredAnalysisRuleListTypeDef = TypedDict(
+    "_RequiredAnalysisRuleListTypeDef",
     {
         "joinColumns": Sequence[str],
         "listColumns": Sequence[str],
     },
 )
+_OptionalAnalysisRuleListTypeDef = TypedDict(
+    "_OptionalAnalysisRuleListTypeDef",
+    {
+        "allowedJoinOperators": Sequence[JoinOperatorType],
+    },
+    total=False,
+)
 
-BatchGetSchemaErrorTypeDef = TypedDict(
-    "BatchGetSchemaErrorTypeDef",
+
+class AnalysisRuleListTypeDef(_RequiredAnalysisRuleListTypeDef, _OptionalAnalysisRuleListTypeDef):
+    pass
+
+
+AnalysisSchemaTypeDef = TypedDict(
+    "AnalysisSchemaTypeDef",
+    {
+        "referencedTables": List[str],
+    },
+    total=False,
+)
+
+AnalysisSourceTypeDef = TypedDict(
+    "AnalysisSourceTypeDef",
     {
+        "text": str,
+    },
+    total=False,
+)
+
+_RequiredAnalysisTemplateSummaryTypeDef = TypedDict(
+    "_RequiredAnalysisTemplateSummaryTypeDef",
+    {
+        "arn": str,
+        "createTime": datetime,
+        "id": str,
         "name": str,
+        "updateTime": datetime,
+        "membershipArn": str,
+        "membershipId": str,
+        "collaborationArn": str,
+        "collaborationId": str,
+    },
+)
+_OptionalAnalysisTemplateSummaryTypeDef = TypedDict(
+    "_OptionalAnalysisTemplateSummaryTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+
+class AnalysisTemplateSummaryTypeDef(
+    _RequiredAnalysisTemplateSummaryTypeDef, _OptionalAnalysisTemplateSummaryTypeDef
+):
+    pass
+
+
+BatchGetCollaborationAnalysisTemplateErrorTypeDef = TypedDict(
+    "BatchGetCollaborationAnalysisTemplateErrorTypeDef",
+    {
+        "arn": str,
         "code": str,
         "message": str,
     },
 )
 
-BatchGetSchemaInputRequestTypeDef = TypedDict(
-    "BatchGetSchemaInputRequestTypeDef",
+BatchGetCollaborationAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "BatchGetCollaborationAnalysisTemplateInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
-        "names": Sequence[str],
+        "analysisTemplateArns": Sequence[str],
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+BatchGetSchemaErrorTypeDef = TypedDict(
+    "BatchGetSchemaErrorTypeDef",
+    {
+        "name": str,
+        "code": str,
+        "message": str,
+    },
+)
+
+BatchGetSchemaInputRequestTypeDef = TypedDict(
+    "BatchGetSchemaInputRequestTypeDef",
+    {
+        "collaborationIdentifier": str,
+        "names": Sequence[str],
+    },
+)
+
+_RequiredCollaborationAnalysisTemplateSummaryTypeDef = TypedDict(
+    "_RequiredCollaborationAnalysisTemplateSummaryTypeDef",
+    {
+        "arn": str,
+        "createTime": datetime,
+        "id": str,
+        "name": str,
+        "updateTime": datetime,
+        "collaborationArn": str,
+        "collaborationId": str,
+        "creatorAccountId": str,
+    },
+)
+_OptionalCollaborationAnalysisTemplateSummaryTypeDef = TypedDict(
+    "_OptionalCollaborationAnalysisTemplateSummaryTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+
+class CollaborationAnalysisTemplateSummaryTypeDef(
+    _RequiredCollaborationAnalysisTemplateSummaryTypeDef,
+    _OptionalCollaborationAnalysisTemplateSummaryTypeDef,
+):
+    pass
+
+
 _RequiredCollaborationSummaryTypeDef = TypedDict(
     "_RequiredCollaborationSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "creatorAccountId": str,
@@ -384,14 +558,22 @@
         "updateTime": datetime,
         "status": MembershipStatusType,
         "memberAbilities": List[MemberAbilityType],
         "queryLogStatus": MembershipQueryLogStatusType,
     },
 )
 
+DeleteAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "DeleteAnalysisTemplateInputRequestTypeDef",
+    {
+        "membershipIdentifier": str,
+        "analysisTemplateIdentifier": str,
+    },
+)
+
 DeleteCollaborationInputRequestTypeDef = TypedDict(
     "DeleteCollaborationInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 
@@ -429,14 +611,30 @@
 DeleteMembershipInputRequestTypeDef = TypedDict(
     "DeleteMembershipInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 
+GetAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "GetAnalysisTemplateInputRequestTypeDef",
+    {
+        "membershipIdentifier": str,
+        "analysisTemplateIdentifier": str,
+    },
+)
+
+GetCollaborationAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "GetCollaborationAnalysisTemplateInputRequestTypeDef",
+    {
+        "collaborationIdentifier": str,
+        "analysisTemplateArn": str,
+    },
+)
+
 GetCollaborationInputRequestTypeDef = TypedDict(
     "GetCollaborationInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 
@@ -509,14 +707,60 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredListAnalysisTemplatesInputRequestTypeDef = TypedDict(
+    "_RequiredListAnalysisTemplatesInputRequestTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListAnalysisTemplatesInputRequestTypeDef = TypedDict(
+    "_OptionalListAnalysisTemplatesInputRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListAnalysisTemplatesInputRequestTypeDef(
+    _RequiredListAnalysisTemplatesInputRequestTypeDef,
+    _OptionalListAnalysisTemplatesInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredListCollaborationAnalysisTemplatesInputRequestTypeDef = TypedDict(
+    "_RequiredListCollaborationAnalysisTemplatesInputRequestTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListCollaborationAnalysisTemplatesInputRequestTypeDef = TypedDict(
+    "_OptionalListCollaborationAnalysisTemplatesInputRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListCollaborationAnalysisTemplatesInputRequestTypeDef(
+    _RequiredListCollaborationAnalysisTemplatesInputRequestTypeDef,
+    _OptionalListCollaborationAnalysisTemplatesInputRequestTypeDef,
+):
+    pass
+
+
 ListCollaborationsInputRequestTypeDef = TypedDict(
     "ListCollaborationsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "memberStatus": FilterableMemberStatusType,
     },
@@ -758,15 +1002,18 @@
     },
 )
 
 ProtectedQuerySQLParametersTypeDef = TypedDict(
     "ProtectedQuerySQLParametersTypeDef",
     {
         "queryString": str,
+        "analysisTemplateArn": str,
+        "parameters": Dict[str, str],
     },
+    total=False,
 )
 
 ProtectedQueryStatisticsTypeDef = TypedDict(
     "ProtectedQueryStatisticsTypeDef",
     {
         "totalDurationInMillis": int,
     },
@@ -785,14 +1032,37 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+_RequiredUpdateAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateAnalysisTemplateInputRequestTypeDef",
+    {
+        "membershipIdentifier": str,
+        "analysisTemplateIdentifier": str,
+    },
+)
+_OptionalUpdateAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateAnalysisTemplateInputRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+
+class UpdateAnalysisTemplateInputRequestTypeDef(
+    _RequiredUpdateAnalysisTemplateInputRequestTypeDef,
+    _OptionalUpdateAnalysisTemplateInputRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateCollaborationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateCollaborationInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalUpdateCollaborationInputRequestTypeDef = TypedDict(
@@ -898,33 +1168,142 @@
         "outputConstraints": Sequence[AggregationConstraintTypeDef],
     },
 )
 _OptionalAnalysisRuleAggregationTypeDef = TypedDict(
     "_OptionalAnalysisRuleAggregationTypeDef",
     {
         "joinRequired": Literal["QUERY_RUNNER"],
+        "allowedJoinOperators": Sequence[JoinOperatorType],
     },
     total=False,
 )
 
 
 class AnalysisRuleAggregationTypeDef(
     _RequiredAnalysisRuleAggregationTypeDef, _OptionalAnalysisRuleAggregationTypeDef
 ):
     pass
 
 
+_RequiredAnalysisTemplateTypeDef = TypedDict(
+    "_RequiredAnalysisTemplateTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "collaborationId": str,
+        "collaborationArn": str,
+        "membershipId": str,
+        "membershipArn": str,
+        "name": str,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "schema": AnalysisSchemaTypeDef,
+        "format": Literal["SQL"],
+        "source": AnalysisSourceTypeDef,
+    },
+)
+_OptionalAnalysisTemplateTypeDef = TypedDict(
+    "_OptionalAnalysisTemplateTypeDef",
+    {
+        "description": str,
+        "analysisParameters": List[AnalysisParameterTypeDef],
+    },
+    total=False,
+)
+
+
+class AnalysisTemplateTypeDef(_RequiredAnalysisTemplateTypeDef, _OptionalAnalysisTemplateTypeDef):
+    pass
+
+
+_RequiredCollaborationAnalysisTemplateTypeDef = TypedDict(
+    "_RequiredCollaborationAnalysisTemplateTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "collaborationId": str,
+        "collaborationArn": str,
+        "creatorAccountId": str,
+        "name": str,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "schema": AnalysisSchemaTypeDef,
+        "format": Literal["SQL"],
+        "source": AnalysisSourceTypeDef,
+    },
+)
+_OptionalCollaborationAnalysisTemplateTypeDef = TypedDict(
+    "_OptionalCollaborationAnalysisTemplateTypeDef",
+    {
+        "description": str,
+        "analysisParameters": List[AnalysisParameterTypeDef],
+    },
+    total=False,
+)
+
+
+class CollaborationAnalysisTemplateTypeDef(
+    _RequiredCollaborationAnalysisTemplateTypeDef, _OptionalCollaborationAnalysisTemplateTypeDef
+):
+    pass
+
+
+_RequiredCreateAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "_RequiredCreateAnalysisTemplateInputRequestTypeDef",
+    {
+        "membershipIdentifier": str,
+        "name": str,
+        "format": Literal["SQL"],
+        "source": AnalysisSourceTypeDef,
+    },
+)
+_OptionalCreateAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "_OptionalCreateAnalysisTemplateInputRequestTypeDef",
+    {
+        "description": str,
+        "tags": Mapping[str, str],
+        "analysisParameters": Sequence[AnalysisParameterTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateAnalysisTemplateInputRequestTypeDef(
+    _RequiredCreateAnalysisTemplateInputRequestTypeDef,
+    _OptionalCreateAnalysisTemplateInputRequestTypeDef,
+):
+    pass
+
+
+ListAnalysisTemplatesOutputTypeDef = TypedDict(
+    "ListAnalysisTemplatesOutputTypeDef",
+    {
+        "nextToken": str,
+        "analysisTemplateSummaries": List[AnalysisTemplateSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListCollaborationAnalysisTemplatesOutputTypeDef = TypedDict(
+    "ListCollaborationAnalysisTemplatesOutputTypeDef",
+    {
+        "nextToken": str,
+        "collaborationAnalysisTemplateSummaries": List[CollaborationAnalysisTemplateSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCollaborationsOutputTypeDef = TypedDict(
     "ListCollaborationsOutputTypeDef",
     {
         "nextToken": str,
         "collaborationList": List[CollaborationSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1086,14 +1465,58 @@
     "TableReferenceTypeDef",
     {
         "glue": GlueTableReferenceTypeDef,
     },
     total=False,
 )
 
+_RequiredListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef = TypedDict(
+    "_RequiredListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef = TypedDict(
+    "_OptionalListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef(
+    _RequiredListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef,
+    _OptionalListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef = TypedDict(
+    "_RequiredListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef = TypedDict(
+    "_OptionalListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef(
+    _RequiredListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef,
+    _OptionalListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef,
+):
+    pass
+
+
 ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
     "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     {
         "memberStatus": FilterableMemberStatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1259,27 +1682,70 @@
 )
 
 AnalysisRulePolicyV1TypeDef = TypedDict(
     "AnalysisRulePolicyV1TypeDef",
     {
         "list": AnalysisRuleListTypeDef,
         "aggregation": AnalysisRuleAggregationTypeDef,
+        "custom": AnalysisRuleCustomTypeDef,
     },
     total=False,
 )
 
 ConfiguredTableAnalysisRulePolicyV1TypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     {
         "list": AnalysisRuleListTypeDef,
         "aggregation": AnalysisRuleAggregationTypeDef,
+        "custom": AnalysisRuleCustomTypeDef,
     },
     total=False,
 )
 
+CreateAnalysisTemplateOutputTypeDef = TypedDict(
+    "CreateAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAnalysisTemplateOutputTypeDef = TypedDict(
+    "GetAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnalysisTemplateOutputTypeDef = TypedDict(
+    "UpdateAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchGetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
+    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
+    {
+        "collaborationAnalysisTemplates": List[CollaborationAnalysisTemplateTypeDef],
+        "errors": List[BatchGetCollaborationAnalysisTemplateErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
+    "GetCollaborationAnalysisTemplateOutputTypeDef",
+    {
+        "collaborationAnalysisTemplate": CollaborationAnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateCollaborationOutputTypeDef = TypedDict(
     "CreateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms/type_defs.pyi` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms/type_defs.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
+    JoinOperatorType,
     MemberAbilityType,
     MembershipQueryLogStatusType,
     MembershipStatusType,
     MemberStatusType,
+    ParameterTypeType,
     ProtectedQueryStatusType,
     ResultFormatType,
     ScalarFunctionsType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -38,44 +40,57 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AggregateColumnTypeDef",
     "AggregationConstraintTypeDef",
+    "AnalysisParameterTypeDef",
+    "AnalysisRuleCustomTypeDef",
     "AnalysisRuleListTypeDef",
+    "AnalysisSchemaTypeDef",
+    "AnalysisSourceTypeDef",
+    "AnalysisTemplateSummaryTypeDef",
+    "BatchGetCollaborationAnalysisTemplateErrorTypeDef",
+    "BatchGetCollaborationAnalysisTemplateInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CollaborationAnalysisTemplateSummaryTypeDef",
     "CollaborationSummaryTypeDef",
     "DataEncryptionMetadataTypeDef",
     "ColumnTypeDef",
     "ConfiguredTableAssociationSummaryTypeDef",
     "ConfiguredTableAssociationTypeDef",
     "ConfiguredTableSummaryTypeDef",
     "MemberSpecificationTypeDef",
     "CreateConfiguredTableAssociationInputRequestTypeDef",
     "CreateMembershipInputRequestTypeDef",
     "MembershipTypeDef",
+    "DeleteAnalysisTemplateInputRequestTypeDef",
     "DeleteCollaborationInputRequestTypeDef",
     "DeleteConfiguredTableAnalysisRuleInputRequestTypeDef",
     "DeleteConfiguredTableAssociationInputRequestTypeDef",
     "DeleteConfiguredTableInputRequestTypeDef",
     "DeleteMemberInputRequestTypeDef",
     "DeleteMembershipInputRequestTypeDef",
+    "GetAnalysisTemplateInputRequestTypeDef",
+    "GetCollaborationAnalysisTemplateInputRequestTypeDef",
     "GetCollaborationInputRequestTypeDef",
     "GetConfiguredTableAnalysisRuleInputRequestTypeDef",
     "GetConfiguredTableAssociationInputRequestTypeDef",
     "GetConfiguredTableInputRequestTypeDef",
     "GetMembershipInputRequestTypeDef",
     "GetProtectedQueryInputRequestTypeDef",
     "GetSchemaAnalysisRuleInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "GlueTableReferenceTypeDef",
     "PaginatorConfigTypeDef",
+    "ListAnalysisTemplatesInputRequestTypeDef",
+    "ListCollaborationAnalysisTemplatesInputRequestTypeDef",
     "ListCollaborationsInputRequestTypeDef",
     "ListConfiguredTableAssociationsInputRequestTypeDef",
     "ListConfiguredTablesInputRequestTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
     "ListMembershipsInputRequestTypeDef",
     "MembershipSummaryTypeDef",
@@ -87,34 +102,42 @@
     "ProtectedQueryErrorTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "UpdateAnalysisTemplateInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
     "AnalysisRuleAggregationTypeDef",
+    "AnalysisTemplateTypeDef",
+    "CollaborationAnalysisTemplateTypeDef",
+    "CreateAnalysisTemplateInputRequestTypeDef",
+    "ListAnalysisTemplatesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "ListCollaborationAnalysisTemplatesOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
     "ListConfiguredTablesOutputTypeDef",
     "CreateCollaborationInputRequestTypeDef",
     "CreateMembershipOutputTypeDef",
     "GetMembershipOutputTypeDef",
     "UpdateMembershipOutputTypeDef",
     "TableReferenceTypeDef",
+    "ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef",
+    "ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef",
     "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
     "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
     "ListMembersInputListMembersPaginateTypeDef",
     "ListMembershipsInputListMembershipsPaginateTypeDef",
     "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
     "ListSchemasInputListSchemasPaginateTypeDef",
@@ -122,14 +145,19 @@
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
+    "CreateAnalysisTemplateOutputTypeDef",
+    "GetAnalysisTemplateOutputTypeDef",
+    "UpdateAnalysisTemplateOutputTypeDef",
+    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
+    "GetCollaborationAnalysisTemplateOutputTypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "BatchGetSchemaOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "ConfiguredTableTypeDef",
     "CreateConfiguredTableInputRequestTypeDef",
@@ -168,50 +196,186 @@
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
 )
 
-AnalysisRuleListTypeDef = TypedDict(
-    "AnalysisRuleListTypeDef",
+_RequiredAnalysisParameterTypeDef = TypedDict(
+    "_RequiredAnalysisParameterTypeDef",
+    {
+        "name": str,
+        "type": ParameterTypeType,
+    },
+)
+_OptionalAnalysisParameterTypeDef = TypedDict(
+    "_OptionalAnalysisParameterTypeDef",
+    {
+        "defaultValue": str,
+    },
+    total=False,
+)
+
+class AnalysisParameterTypeDef(
+    _RequiredAnalysisParameterTypeDef, _OptionalAnalysisParameterTypeDef
+):
+    pass
+
+_RequiredAnalysisRuleCustomTypeDef = TypedDict(
+    "_RequiredAnalysisRuleCustomTypeDef",
+    {
+        "allowedAnalyses": Sequence[str],
+    },
+)
+_OptionalAnalysisRuleCustomTypeDef = TypedDict(
+    "_OptionalAnalysisRuleCustomTypeDef",
+    {
+        "allowedAnalysisProviders": Sequence[str],
+    },
+    total=False,
+)
+
+class AnalysisRuleCustomTypeDef(
+    _RequiredAnalysisRuleCustomTypeDef, _OptionalAnalysisRuleCustomTypeDef
+):
+    pass
+
+_RequiredAnalysisRuleListTypeDef = TypedDict(
+    "_RequiredAnalysisRuleListTypeDef",
     {
         "joinColumns": Sequence[str],
         "listColumns": Sequence[str],
     },
 )
+_OptionalAnalysisRuleListTypeDef = TypedDict(
+    "_OptionalAnalysisRuleListTypeDef",
+    {
+        "allowedJoinOperators": Sequence[JoinOperatorType],
+    },
+    total=False,
+)
 
-BatchGetSchemaErrorTypeDef = TypedDict(
-    "BatchGetSchemaErrorTypeDef",
+class AnalysisRuleListTypeDef(_RequiredAnalysisRuleListTypeDef, _OptionalAnalysisRuleListTypeDef):
+    pass
+
+AnalysisSchemaTypeDef = TypedDict(
+    "AnalysisSchemaTypeDef",
+    {
+        "referencedTables": List[str],
+    },
+    total=False,
+)
+
+AnalysisSourceTypeDef = TypedDict(
+    "AnalysisSourceTypeDef",
+    {
+        "text": str,
+    },
+    total=False,
+)
+
+_RequiredAnalysisTemplateSummaryTypeDef = TypedDict(
+    "_RequiredAnalysisTemplateSummaryTypeDef",
     {
+        "arn": str,
+        "createTime": datetime,
+        "id": str,
         "name": str,
+        "updateTime": datetime,
+        "membershipArn": str,
+        "membershipId": str,
+        "collaborationArn": str,
+        "collaborationId": str,
+    },
+)
+_OptionalAnalysisTemplateSummaryTypeDef = TypedDict(
+    "_OptionalAnalysisTemplateSummaryTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class AnalysisTemplateSummaryTypeDef(
+    _RequiredAnalysisTemplateSummaryTypeDef, _OptionalAnalysisTemplateSummaryTypeDef
+):
+    pass
+
+BatchGetCollaborationAnalysisTemplateErrorTypeDef = TypedDict(
+    "BatchGetCollaborationAnalysisTemplateErrorTypeDef",
+    {
+        "arn": str,
         "code": str,
         "message": str,
     },
 )
 
-BatchGetSchemaInputRequestTypeDef = TypedDict(
-    "BatchGetSchemaInputRequestTypeDef",
+BatchGetCollaborationAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "BatchGetCollaborationAnalysisTemplateInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
-        "names": Sequence[str],
+        "analysisTemplateArns": Sequence[str],
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+BatchGetSchemaErrorTypeDef = TypedDict(
+    "BatchGetSchemaErrorTypeDef",
+    {
+        "name": str,
+        "code": str,
+        "message": str,
+    },
+)
+
+BatchGetSchemaInputRequestTypeDef = TypedDict(
+    "BatchGetSchemaInputRequestTypeDef",
+    {
+        "collaborationIdentifier": str,
+        "names": Sequence[str],
+    },
+)
+
+_RequiredCollaborationAnalysisTemplateSummaryTypeDef = TypedDict(
+    "_RequiredCollaborationAnalysisTemplateSummaryTypeDef",
+    {
+        "arn": str,
+        "createTime": datetime,
+        "id": str,
+        "name": str,
+        "updateTime": datetime,
+        "collaborationArn": str,
+        "collaborationId": str,
+        "creatorAccountId": str,
+    },
+)
+_OptionalCollaborationAnalysisTemplateSummaryTypeDef = TypedDict(
+    "_OptionalCollaborationAnalysisTemplateSummaryTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class CollaborationAnalysisTemplateSummaryTypeDef(
+    _RequiredCollaborationAnalysisTemplateSummaryTypeDef,
+    _OptionalCollaborationAnalysisTemplateSummaryTypeDef,
+):
+    pass
+
 _RequiredCollaborationSummaryTypeDef = TypedDict(
     "_RequiredCollaborationSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "creatorAccountId": str,
@@ -375,14 +539,22 @@
         "updateTime": datetime,
         "status": MembershipStatusType,
         "memberAbilities": List[MemberAbilityType],
         "queryLogStatus": MembershipQueryLogStatusType,
     },
 )
 
+DeleteAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "DeleteAnalysisTemplateInputRequestTypeDef",
+    {
+        "membershipIdentifier": str,
+        "analysisTemplateIdentifier": str,
+    },
+)
+
 DeleteCollaborationInputRequestTypeDef = TypedDict(
     "DeleteCollaborationInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 
@@ -420,14 +592,30 @@
 DeleteMembershipInputRequestTypeDef = TypedDict(
     "DeleteMembershipInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 
+GetAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "GetAnalysisTemplateInputRequestTypeDef",
+    {
+        "membershipIdentifier": str,
+        "analysisTemplateIdentifier": str,
+    },
+)
+
+GetCollaborationAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "GetCollaborationAnalysisTemplateInputRequestTypeDef",
+    {
+        "collaborationIdentifier": str,
+        "analysisTemplateArn": str,
+    },
+)
+
 GetCollaborationInputRequestTypeDef = TypedDict(
     "GetCollaborationInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 
@@ -500,14 +688,56 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredListAnalysisTemplatesInputRequestTypeDef = TypedDict(
+    "_RequiredListAnalysisTemplatesInputRequestTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListAnalysisTemplatesInputRequestTypeDef = TypedDict(
+    "_OptionalListAnalysisTemplatesInputRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListAnalysisTemplatesInputRequestTypeDef(
+    _RequiredListAnalysisTemplatesInputRequestTypeDef,
+    _OptionalListAnalysisTemplatesInputRequestTypeDef,
+):
+    pass
+
+_RequiredListCollaborationAnalysisTemplatesInputRequestTypeDef = TypedDict(
+    "_RequiredListCollaborationAnalysisTemplatesInputRequestTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListCollaborationAnalysisTemplatesInputRequestTypeDef = TypedDict(
+    "_OptionalListCollaborationAnalysisTemplatesInputRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListCollaborationAnalysisTemplatesInputRequestTypeDef(
+    _RequiredListCollaborationAnalysisTemplatesInputRequestTypeDef,
+    _OptionalListCollaborationAnalysisTemplatesInputRequestTypeDef,
+):
+    pass
+
 ListCollaborationsInputRequestTypeDef = TypedDict(
     "ListCollaborationsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "memberStatus": FilterableMemberStatusType,
     },
@@ -735,15 +965,18 @@
     },
 )
 
 ProtectedQuerySQLParametersTypeDef = TypedDict(
     "ProtectedQuerySQLParametersTypeDef",
     {
         "queryString": str,
+        "analysisTemplateArn": str,
+        "parameters": Dict[str, str],
     },
+    total=False,
 )
 
 ProtectedQueryStatisticsTypeDef = TypedDict(
     "ProtectedQueryStatisticsTypeDef",
     {
         "totalDurationInMillis": int,
     },
@@ -762,14 +995,35 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+_RequiredUpdateAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateAnalysisTemplateInputRequestTypeDef",
+    {
+        "membershipIdentifier": str,
+        "analysisTemplateIdentifier": str,
+    },
+)
+_OptionalUpdateAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateAnalysisTemplateInputRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class UpdateAnalysisTemplateInputRequestTypeDef(
+    _RequiredUpdateAnalysisTemplateInputRequestTypeDef,
+    _OptionalUpdateAnalysisTemplateInputRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateCollaborationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateCollaborationInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalUpdateCollaborationInputRequestTypeDef = TypedDict(
@@ -867,31 +1121,134 @@
         "outputConstraints": Sequence[AggregationConstraintTypeDef],
     },
 )
 _OptionalAnalysisRuleAggregationTypeDef = TypedDict(
     "_OptionalAnalysisRuleAggregationTypeDef",
     {
         "joinRequired": Literal["QUERY_RUNNER"],
+        "allowedJoinOperators": Sequence[JoinOperatorType],
     },
     total=False,
 )
 
 class AnalysisRuleAggregationTypeDef(
     _RequiredAnalysisRuleAggregationTypeDef, _OptionalAnalysisRuleAggregationTypeDef
 ):
     pass
 
+_RequiredAnalysisTemplateTypeDef = TypedDict(
+    "_RequiredAnalysisTemplateTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "collaborationId": str,
+        "collaborationArn": str,
+        "membershipId": str,
+        "membershipArn": str,
+        "name": str,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "schema": AnalysisSchemaTypeDef,
+        "format": Literal["SQL"],
+        "source": AnalysisSourceTypeDef,
+    },
+)
+_OptionalAnalysisTemplateTypeDef = TypedDict(
+    "_OptionalAnalysisTemplateTypeDef",
+    {
+        "description": str,
+        "analysisParameters": List[AnalysisParameterTypeDef],
+    },
+    total=False,
+)
+
+class AnalysisTemplateTypeDef(_RequiredAnalysisTemplateTypeDef, _OptionalAnalysisTemplateTypeDef):
+    pass
+
+_RequiredCollaborationAnalysisTemplateTypeDef = TypedDict(
+    "_RequiredCollaborationAnalysisTemplateTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "collaborationId": str,
+        "collaborationArn": str,
+        "creatorAccountId": str,
+        "name": str,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "schema": AnalysisSchemaTypeDef,
+        "format": Literal["SQL"],
+        "source": AnalysisSourceTypeDef,
+    },
+)
+_OptionalCollaborationAnalysisTemplateTypeDef = TypedDict(
+    "_OptionalCollaborationAnalysisTemplateTypeDef",
+    {
+        "description": str,
+        "analysisParameters": List[AnalysisParameterTypeDef],
+    },
+    total=False,
+)
+
+class CollaborationAnalysisTemplateTypeDef(
+    _RequiredCollaborationAnalysisTemplateTypeDef, _OptionalCollaborationAnalysisTemplateTypeDef
+):
+    pass
+
+_RequiredCreateAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "_RequiredCreateAnalysisTemplateInputRequestTypeDef",
+    {
+        "membershipIdentifier": str,
+        "name": str,
+        "format": Literal["SQL"],
+        "source": AnalysisSourceTypeDef,
+    },
+)
+_OptionalCreateAnalysisTemplateInputRequestTypeDef = TypedDict(
+    "_OptionalCreateAnalysisTemplateInputRequestTypeDef",
+    {
+        "description": str,
+        "tags": Mapping[str, str],
+        "analysisParameters": Sequence[AnalysisParameterTypeDef],
+    },
+    total=False,
+)
+
+class CreateAnalysisTemplateInputRequestTypeDef(
+    _RequiredCreateAnalysisTemplateInputRequestTypeDef,
+    _OptionalCreateAnalysisTemplateInputRequestTypeDef,
+):
+    pass
+
+ListAnalysisTemplatesOutputTypeDef = TypedDict(
+    "ListAnalysisTemplatesOutputTypeDef",
+    {
+        "nextToken": str,
+        "analysisTemplateSummaries": List[AnalysisTemplateSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListCollaborationAnalysisTemplatesOutputTypeDef = TypedDict(
+    "ListCollaborationAnalysisTemplatesOutputTypeDef",
+    {
+        "nextToken": str,
+        "collaborationAnalysisTemplateSummaries": List[CollaborationAnalysisTemplateSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCollaborationsOutputTypeDef = TypedDict(
     "ListCollaborationsOutputTypeDef",
     {
         "nextToken": str,
         "collaborationList": List[CollaborationSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1047,14 +1404,54 @@
     "TableReferenceTypeDef",
     {
         "glue": GlueTableReferenceTypeDef,
     },
     total=False,
 )
 
+_RequiredListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef = TypedDict(
+    "_RequiredListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef = TypedDict(
+    "_OptionalListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef(
+    _RequiredListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef,
+    _OptionalListAnalysisTemplatesInputListAnalysisTemplatesPaginateTypeDef,
+):
+    pass
+
+_RequiredListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef = TypedDict(
+    "_RequiredListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef = TypedDict(
+    "_OptionalListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef(
+    _RequiredListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef,
+    _OptionalListCollaborationAnalysisTemplatesInputListCollaborationAnalysisTemplatesPaginateTypeDef,
+):
+    pass
+
 ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
     "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     {
         "memberStatus": FilterableMemberStatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1212,27 +1609,70 @@
 )
 
 AnalysisRulePolicyV1TypeDef = TypedDict(
     "AnalysisRulePolicyV1TypeDef",
     {
         "list": AnalysisRuleListTypeDef,
         "aggregation": AnalysisRuleAggregationTypeDef,
+        "custom": AnalysisRuleCustomTypeDef,
     },
     total=False,
 )
 
 ConfiguredTableAnalysisRulePolicyV1TypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     {
         "list": AnalysisRuleListTypeDef,
         "aggregation": AnalysisRuleAggregationTypeDef,
+        "custom": AnalysisRuleCustomTypeDef,
     },
     total=False,
 )
 
+CreateAnalysisTemplateOutputTypeDef = TypedDict(
+    "CreateAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAnalysisTemplateOutputTypeDef = TypedDict(
+    "GetAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnalysisTemplateOutputTypeDef = TypedDict(
+    "UpdateAnalysisTemplateOutputTypeDef",
+    {
+        "analysisTemplate": AnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchGetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
+    "BatchGetCollaborationAnalysisTemplateOutputTypeDef",
+    {
+        "collaborationAnalysisTemplates": List[CollaborationAnalysisTemplateTypeDef],
+        "errors": List[BatchGetCollaborationAnalysisTemplateErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCollaborationAnalysisTemplateOutputTypeDef = TypedDict(
+    "GetCollaborationAnalysisTemplateOutputTypeDef",
+    {
+        "collaborationAnalysisTemplate": CollaborationAnalysisTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateCollaborationOutputTypeDef = TypedDict(
     "CreateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms.egg-info/PKG-INFO` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cleanrooms
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.CleanRoomsService 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.CleanRoomsService 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanrooms)](https://pepy.tech/project/types-aiobotocore-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CleanRoomsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[aiobotocore.CleanRoomsService 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -272,14 +272,16 @@
 all paginators.
 
 ```python
 from aiobotocore.session import get_session
 
 from types_aiobotocore_cleanrooms import CleanRoomsServiceClient
 from types_aiobotocore_cleanrooms.paginator import (
+    ListAnalysisTemplatesPaginator,
+    ListCollaborationAnalysisTemplatesPaginator,
     ListCollaborationsPaginator,
     ListConfiguredTableAssociationsPaginator,
     ListConfiguredTablesPaginator,
     ListMembersPaginator,
     ListMembershipsPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
@@ -287,14 +289,20 @@
 
 session = get_session()
 async with session.create_client("cleanrooms") as client:
     client: CleanRoomsServiceClient
 
     # Explicit type annotations are optional here
     # Types should be correctly discovered by mypy and IDEs
+    list_analysis_templates_paginator: ListAnalysisTemplatesPaginator = client.get_paginator(
+        "list_analysis_templates"
+    )
+    list_collaboration_analysis_templates_paginator: ListCollaborationAnalysisTemplatesPaginator = (
+        client.get_paginator("list_collaboration_analysis_templates")
+    )
     list_collaborations_paginator: ListCollaborationsPaginator = client.get_paginator(
         "list_collaborations"
     )
     list_configured_table_associations_paginator: ListConfiguredTableAssociationsPaginator = (
         client.get_paginator("list_configured_table_associations")
     )
     list_configured_tables_paginator: ListConfiguredTablesPaginator = client.get_paginator(
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post3/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt` & `types-aiobotocore-cleanrooms-2.5.4/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

