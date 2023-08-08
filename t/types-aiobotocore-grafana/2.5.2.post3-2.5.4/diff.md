# Comparing `tmp/types-aiobotocore-grafana-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-grafana-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-grafana-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-grafana-2.5.4.tar", last modified: Tue Aug  8 01:23:47 2023, max compression
```

## Comparing `types-aiobotocore-grafana-2.5.2.post3.tar` & `types-aiobotocore-grafana-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.975887 types-aiobotocore-grafana-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-08-04 12:37:46.975887 types-aiobotocore-grafana-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:46.975887 types-aiobotocore-grafana-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 12:24:36.000000 types-aiobotocore-grafana-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.975887 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18347 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19341 2023-08-04 12:24:39.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19318 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:38.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:46.975887 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-08-04 12:37:46.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:37:46.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:46.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:46.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:37:46.000000 types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.606726 types-aiobotocore-grafana-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-08-08 01:23:47.606726 types-aiobotocore-grafana-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:23:47.606726 types-aiobotocore-grafana-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.598726 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19367 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20559 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20534 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:11:58.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:23:47.606726 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-08-08 01:23:47.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-08 01:23:47.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:47.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:23:47.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:23:47.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 01:23:47.000000 types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/LICENSE` & `types-aiobotocore-grafana-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-grafana-2.5.2.post3/PKG-INFO` & `types-aiobotocore-grafana-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-grafana
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ManagedGrafana 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ManagedGrafana 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-grafana.svg?color=blue)](https://pypi.org/project/types-aiobotocore-grafana)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-grafana)](https://pepy.tech/project/types-aiobotocore-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedGrafana 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[aiobotocore.ManagedGrafana 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -271,23 +271,28 @@
 `types_aiobotocore_grafana.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from aiobotocore.session import get_session
 
 from types_aiobotocore_grafana import ManagedGrafanaClient
-from types_aiobotocore_grafana.paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from types_aiobotocore_grafana.paginator import (
+    ListPermissionsPaginator,
+    ListVersionsPaginator,
+    ListWorkspacesPaginator,
+)
 
 session = get_session()
 async with session.create_client("grafana") as client:
     client: ManagedGrafanaClient
 
     # Explicit type annotations are optional here
     # Types should be correctly discovered by mypy and IDEs
     list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+    list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
     list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
 ```
 
 <a id="literals"></a>
 
 ### Literals
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/README.md` & `types-aiobotocore-grafana-2.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-grafana.svg?color=blue)](https://pypi.org/project/types-aiobotocore-grafana)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-grafana)](https://pepy.tech/project/types-aiobotocore-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedGrafana 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[aiobotocore.ManagedGrafana 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -239,23 +239,28 @@
 `types_aiobotocore_grafana.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from aiobotocore.session import get_session
 
 from types_aiobotocore_grafana import ManagedGrafanaClient
-from types_aiobotocore_grafana.paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from types_aiobotocore_grafana.paginator import (
+    ListPermissionsPaginator,
+    ListVersionsPaginator,
+    ListWorkspacesPaginator,
+)
 
 session = get_session()
 async with session.create_client("grafana") as client:
     client: ManagedGrafanaClient
 
     # Explicit type annotations are optional here
     # Types should be correctly discovered by mypy and IDEs
     list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+    list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
     list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
 ```
 
 <a id="literals"></a>
 
 ### Literals
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/setup.py` & `types-aiobotocore-grafana-2.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-grafana",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_grafana"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ManagedGrafana 2.5.2 service generated with"
+        "Type annotations for aiobotocore.ManagedGrafana 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/__init__.py` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,28 +4,36 @@
 Usage::
 
     ```python
     from aiobotocore.session import get_session
     from types_aiobotocore_grafana import (
         Client,
         ListPermissionsPaginator,
+        ListVersionsPaginator,
         ListWorkspacesPaginator,
         ManagedGrafanaClient,
     )
 
     session = get_session()
     async with session.create_client("grafana") as client:
         client: ManagedGrafanaClient
         ...
 
 
     list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+    list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
     list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
     ```
 """
 from .client import ManagedGrafanaClient
-from .paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from .paginator import ListPermissionsPaginator, ListVersionsPaginator, ListWorkspacesPaginator
 
 Client = ManagedGrafanaClient
 
 
-__all__ = ("Client", "ListPermissionsPaginator", "ListWorkspacesPaginator", "ManagedGrafanaClient")
+__all__ = (
+    "Client",
+    "ListPermissionsPaginator",
+    "ListVersionsPaginator",
+    "ListWorkspacesPaginator",
+    "ManagedGrafanaClient",
+)
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/__init__.pyi` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/__init__.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -4,27 +4,35 @@
 Usage::
 
     ```python
     from aiobotocore.session import get_session
     from types_aiobotocore_grafana import (
         Client,
         ListPermissionsPaginator,
+        ListVersionsPaginator,
         ListWorkspacesPaginator,
         ManagedGrafanaClient,
     )
 
     session = get_session()
     async with session.create_client("grafana") as client:
         client: ManagedGrafanaClient
         ...
 
 
     list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+    list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
     list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
     ```
 """
 from .client import ManagedGrafanaClient
-from .paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from .paginator import ListPermissionsPaginator, ListVersionsPaginator, ListWorkspacesPaginator
 
 Client = ManagedGrafanaClient
 
-__all__ = ("Client", "ListPermissionsPaginator", "ListWorkspacesPaginator", "ManagedGrafanaClient")
+__all__ = (
+    "Client",
+    "ListPermissionsPaginator",
+    "ListVersionsPaginator",
+    "ListWorkspacesPaginator",
+    "ManagedGrafanaClient",
+)
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/client.py` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,27 +24,28 @@
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
     UserTypeType,
 )
-from .paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from .paginator import ListPermissionsPaginator, ListVersionsPaginator, ListWorkspacesPaginator
 from .type_defs import (
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceApiKeyResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     NetworkAccessConfigurationTypeDef,
     SamlConfigurationTypeDef,
     UpdateInstructionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
@@ -52,37 +53,33 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ManagedGrafanaClient",)
 
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
 class ManagedGrafanaClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/)
     """
 
     meta: ClientMeta
@@ -91,41 +88,37 @@
     def exceptions(self) -> Exceptions:
         """
         ManagedGrafanaClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#exceptions)
         """
-
     async def associate_license(
         self, *, licenseType: LicenseTypeType, workspaceId: str
     ) -> AssociateLicenseResponseTypeDef:
         """
         Assigns a Grafana Enterprise license to a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.associate_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#associate_license)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#close)
         """
-
     async def create_workspace(
         self,
         *,
         accountAccessType: AccountAccessTypeType,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         permissionType: PermissionTypeType,
         clientToken: str = ...,
@@ -145,96 +138,87 @@
     ) -> CreateWorkspaceResponseTypeDef:
         """
         Creates a *workspace*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#create_workspace)
         """
-
     async def create_workspace_api_key(
         self, *, keyName: str, keyRole: str, secondsToLive: int, workspaceId: str
     ) -> CreateWorkspaceApiKeyResponseTypeDef:
         """
         Creates a Grafana API key for the workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace_api_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#create_workspace_api_key)
         """
-
     async def delete_workspace(self, *, workspaceId: str) -> DeleteWorkspaceResponseTypeDef:
         """
         Deletes an Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#delete_workspace)
         """
-
     async def delete_workspace_api_key(
         self, *, keyName: str, workspaceId: str
     ) -> DeleteWorkspaceApiKeyResponseTypeDef:
         """
         Deletes a Grafana API key for the workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace_api_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#delete_workspace_api_key)
         """
-
     async def describe_workspace(self, *, workspaceId: str) -> DescribeWorkspaceResponseTypeDef:
         """
         Displays information about one Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.describe_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#describe_workspace)
         """
-
     async def describe_workspace_authentication(
         self, *, workspaceId: str
     ) -> DescribeWorkspaceAuthenticationResponseTypeDef:
         """
         Displays information about the authentication methods used in one Amazon Managed
         Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.describe_workspace_authentication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#describe_workspace_authentication)
         """
-
     async def describe_workspace_configuration(
         self, *, workspaceId: str
     ) -> DescribeWorkspaceConfigurationResponseTypeDef:
         """
         Gets the current configuration string for the given workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.describe_workspace_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#describe_workspace_configuration)
         """
-
     async def disassociate_license(
         self, *, licenseType: LicenseTypeType, workspaceId: str
     ) -> DisassociateLicenseResponseTypeDef:
         """
         Removes the Grafana Enterprise license from a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.disassociate_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#disassociate_license)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#generate_presigned_url)
         """
-
     async def list_permissions(
         self,
         *,
         workspaceId: str,
         groupId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -244,65 +228,68 @@
         """
         Lists the users and groups who have the Grafana `Admin` and `Editor` roles in
         this workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#list_permissions)
         """
-
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         The `ListTagsForResource` operation returns the tags that are associated with
         the Amazon Managed Service for Grafana resource specified by the `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#list_tags_for_resource)
         """
+    async def list_versions(
+        self, *, maxResults: int = ..., nextToken: str = ..., workspaceId: str = ...
+    ) -> ListVersionsResponseTypeDef:
+        """
+        Lists available versions of Grafana.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_versions)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#list_versions)
+        """
     async def list_workspaces(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Returns a list of Amazon Managed Grafana workspaces in the account, with some
         information about each workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#list_workspaces)
         """
-
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         The `TagResource` operation associates tags with an Amazon Managed Grafana
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#tag_resource)
         """
-
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         The `UntagResource` operation removes the association of the tag with the Amazon
         Managed Grafana resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#untag_resource)
         """
-
     async def update_permissions(
         self, *, updateInstructionBatch: Sequence[UpdateInstructionTypeDef], workspaceId: str
     ) -> UpdatePermissionsResponseTypeDef:
         """
         Updates which users in a workspace have the Grafana `Admin` or `Editor` roles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_permissions)
         """
-
     async def update_workspace(
         self,
         *,
         workspaceId: str,
         accountAccessType: AccountAccessTypeType = ...,
         networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
         organizationRoleName: str = ...,
@@ -320,61 +307,61 @@
     ) -> UpdateWorkspaceResponseTypeDef:
         """
         Modifies an existing Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_workspace)
         """
-
     async def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
         samlConfiguration: SamlConfigurationTypeDef = ...
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_workspace_authentication)
         """
-
     async def update_workspace_configuration(
-        self, *, configuration: str, workspaceId: str
+        self, *, configuration: str, workspaceId: str, grafanaVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the configuration string for the given workspace See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/grafana-2020-08-18/UpdateWorkspaceConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_workspace_configuration)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_permissions"]
     ) -> ListPermissionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#get_paginator)
         """
-
+    @overload
+    def get_paginator(self, operation_name: Literal["list_versions"]) -> ListVersionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#get_paginator)
+        """
     @overload
     def get_paginator(self, operation_name: Literal["list_workspaces"]) -> ListWorkspacesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "ManagedGrafanaClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/)
         """
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/client.pyi` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,27 +24,28 @@
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
     UserTypeType,
 )
-from .paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from .paginator import ListPermissionsPaginator, ListVersionsPaginator, ListWorkspacesPaginator
 from .type_defs import (
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceApiKeyResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     NetworkAccessConfigurationTypeDef,
     SamlConfigurationTypeDef,
     UpdateInstructionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
@@ -52,33 +53,37 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("ManagedGrafanaClient",)
 
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
 class ManagedGrafanaClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/)
     """
 
     meta: ClientMeta
@@ -87,37 +92,41 @@
     def exceptions(self) -> Exceptions:
         """
         ManagedGrafanaClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#exceptions)
         """
+
     async def associate_license(
         self, *, licenseType: LicenseTypeType, workspaceId: str
     ) -> AssociateLicenseResponseTypeDef:
         """
         Assigns a Grafana Enterprise license to a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.associate_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#associate_license)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#close)
         """
+
     async def create_workspace(
         self,
         *,
         accountAccessType: AccountAccessTypeType,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         permissionType: PermissionTypeType,
         clientToken: str = ...,
@@ -137,87 +146,96 @@
     ) -> CreateWorkspaceResponseTypeDef:
         """
         Creates a *workspace*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#create_workspace)
         """
+
     async def create_workspace_api_key(
         self, *, keyName: str, keyRole: str, secondsToLive: int, workspaceId: str
     ) -> CreateWorkspaceApiKeyResponseTypeDef:
         """
         Creates a Grafana API key for the workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.create_workspace_api_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#create_workspace_api_key)
         """
+
     async def delete_workspace(self, *, workspaceId: str) -> DeleteWorkspaceResponseTypeDef:
         """
         Deletes an Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#delete_workspace)
         """
+
     async def delete_workspace_api_key(
         self, *, keyName: str, workspaceId: str
     ) -> DeleteWorkspaceApiKeyResponseTypeDef:
         """
         Deletes a Grafana API key for the workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.delete_workspace_api_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#delete_workspace_api_key)
         """
+
     async def describe_workspace(self, *, workspaceId: str) -> DescribeWorkspaceResponseTypeDef:
         """
         Displays information about one Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.describe_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#describe_workspace)
         """
+
     async def describe_workspace_authentication(
         self, *, workspaceId: str
     ) -> DescribeWorkspaceAuthenticationResponseTypeDef:
         """
         Displays information about the authentication methods used in one Amazon Managed
         Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.describe_workspace_authentication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#describe_workspace_authentication)
         """
+
     async def describe_workspace_configuration(
         self, *, workspaceId: str
     ) -> DescribeWorkspaceConfigurationResponseTypeDef:
         """
         Gets the current configuration string for the given workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.describe_workspace_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#describe_workspace_configuration)
         """
+
     async def disassociate_license(
         self, *, licenseType: LicenseTypeType, workspaceId: str
     ) -> DisassociateLicenseResponseTypeDef:
         """
         Removes the Grafana Enterprise license from a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.disassociate_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#disassociate_license)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#generate_presigned_url)
         """
+
     async def list_permissions(
         self,
         *,
         workspaceId: str,
         groupId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -227,59 +245,75 @@
         """
         Lists the users and groups who have the Grafana `Admin` and `Editor` roles in
         this workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#list_permissions)
         """
+
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         The `ListTagsForResource` operation returns the tags that are associated with
         the Amazon Managed Service for Grafana resource specified by the `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#list_tags_for_resource)
         """
+
+    async def list_versions(
+        self, *, maxResults: int = ..., nextToken: str = ..., workspaceId: str = ...
+    ) -> ListVersionsResponseTypeDef:
+        """
+        Lists available versions of Grafana.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_versions)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#list_versions)
+        """
+
     async def list_workspaces(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Returns a list of Amazon Managed Grafana workspaces in the account, with some
         information about each workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#list_workspaces)
         """
+
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         The `TagResource` operation associates tags with an Amazon Managed Grafana
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#tag_resource)
         """
+
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         The `UntagResource` operation removes the association of the tag with the Amazon
         Managed Grafana resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#untag_resource)
         """
+
     async def update_permissions(
         self, *, updateInstructionBatch: Sequence[UpdateInstructionTypeDef], workspaceId: str
     ) -> UpdatePermissionsResponseTypeDef:
         """
         Updates which users in a workspace have the Grafana `Admin` or `Editor` roles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_permissions)
         """
+
     async def update_workspace(
         self,
         *,
         workspaceId: str,
         accountAccessType: AccountAccessTypeType = ...,
         networkAccessControl: NetworkAccessConfigurationTypeDef = ...,
         organizationRoleName: str = ...,
@@ -297,55 +331,68 @@
     ) -> UpdateWorkspaceResponseTypeDef:
         """
         Modifies an existing Amazon Managed Grafana workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_workspace)
         """
+
     async def update_workspace_authentication(
         self,
         *,
         authenticationProviders: Sequence[AuthenticationProviderTypesType],
         workspaceId: str,
         samlConfiguration: SamlConfigurationTypeDef = ...
     ) -> UpdateWorkspaceAuthenticationResponseTypeDef:
         """
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_workspace_authentication)
         """
+
     async def update_workspace_configuration(
-        self, *, configuration: str, workspaceId: str
+        self, *, configuration: str, workspaceId: str, grafanaVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the configuration string for the given workspace See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/grafana-2020-08-18/UpdateWorkspaceConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#update_workspace_configuration)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_permissions"]
     ) -> ListPermissionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#get_paginator)
         """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_versions"]) -> ListVersionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#get_paginator)
+        """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_workspaces"]) -> ListWorkspacesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "ManagedGrafanaClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/client/)
         """
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/literals.py` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 __all__ = (
     "AccountAccessTypeType",
     "AuthenticationProviderTypesType",
     "DataSourceTypeType",
     "LicenseTypeType",
     "ListPermissionsPaginatorName",
+    "ListVersionsPaginatorName",
     "ListWorkspacesPaginatorName",
     "NotificationDestinationTypeType",
     "PermissionTypeType",
     "RoleType",
     "SamlConfigurationStatusType",
     "UpdateActionType",
     "UserTypeType",
@@ -52,14 +53,15 @@
     "SITEWISE",
     "TIMESTREAM",
     "TWINMAKER",
     "XRAY",
 ]
 LicenseTypeType = Literal["ENTERPRISE", "ENTERPRISE_FREE_TRIAL"]
 ListPermissionsPaginatorName = Literal["list_permissions"]
+ListVersionsPaginatorName = Literal["list_versions"]
 ListWorkspacesPaginatorName = Literal["list_workspaces"]
 NotificationDestinationTypeType = Literal["SNS"]
 PermissionTypeType = Literal["CUSTOMER_MANAGED", "SERVICE_MANAGED"]
 RoleType = Literal["ADMIN", "EDITOR", "VIEWER"]
 SamlConfigurationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
 UpdateActionType = Literal["ADD", "REVOKE"]
 UserTypeType = Literal["SSO_GROUP", "SSO_USER"]
@@ -71,14 +73,16 @@
     "DELETION_FAILED",
     "FAILED",
     "LICENSE_REMOVAL_FAILED",
     "UPDATE_FAILED",
     "UPDATING",
     "UPGRADE_FAILED",
     "UPGRADING",
+    "VERSION_UPDATE_FAILED",
+    "VERSION_UPDATING",
 ]
 ManagedGrafanaServiceName = Literal["grafana"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -88,14 +92,15 @@
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
@@ -191,14 +196,15 @@
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
@@ -277,26 +283,28 @@
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
@@ -436,15 +444,15 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal["list_permissions", "list_workspaces"]
+PaginatorName = Literal["list_permissions", "list_versions", "list_workspaces"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-west-1",
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/literals.pyi` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 __all__ = (
     "AccountAccessTypeType",
     "AuthenticationProviderTypesType",
     "DataSourceTypeType",
     "LicenseTypeType",
     "ListPermissionsPaginatorName",
+    "ListVersionsPaginatorName",
     "ListWorkspacesPaginatorName",
     "NotificationDestinationTypeType",
     "PermissionTypeType",
     "RoleType",
     "SamlConfigurationStatusType",
     "UpdateActionType",
     "UserTypeType",
@@ -50,14 +51,15 @@
     "SITEWISE",
     "TIMESTREAM",
     "TWINMAKER",
     "XRAY",
 ]
 LicenseTypeType = Literal["ENTERPRISE", "ENTERPRISE_FREE_TRIAL"]
 ListPermissionsPaginatorName = Literal["list_permissions"]
+ListVersionsPaginatorName = Literal["list_versions"]
 ListWorkspacesPaginatorName = Literal["list_workspaces"]
 NotificationDestinationTypeType = Literal["SNS"]
 PermissionTypeType = Literal["CUSTOMER_MANAGED", "SERVICE_MANAGED"]
 RoleType = Literal["ADMIN", "EDITOR", "VIEWER"]
 SamlConfigurationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
 UpdateActionType = Literal["ADD", "REVOKE"]
 UserTypeType = Literal["SSO_GROUP", "SSO_USER"]
@@ -69,14 +71,16 @@
     "DELETION_FAILED",
     "FAILED",
     "LICENSE_REMOVAL_FAILED",
     "UPDATE_FAILED",
     "UPDATING",
     "UPGRADE_FAILED",
     "UPGRADING",
+    "VERSION_UPDATE_FAILED",
+    "VERSION_UPDATING",
 ]
 ManagedGrafanaServiceName = Literal["grafana"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -86,14 +90,15 @@
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
@@ -189,14 +194,15 @@
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
@@ -275,26 +281,28 @@
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
@@ -434,15 +442,15 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal["list_permissions", "list_workspaces"]
+PaginatorName = Literal["list_permissions", "list_versions", "list_workspaces"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-west-1",
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/paginator.py` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/paginator.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -7,50 +7,50 @@
 
     ```python
     from aiobotocore.session import get_session
 
     from types_aiobotocore_grafana.client import ManagedGrafanaClient
     from types_aiobotocore_grafana.paginator import (
         ListPermissionsPaginator,
+        ListVersionsPaginator,
         ListWorkspacesPaginator,
     )
 
     session = get_session()
     with session.create_client("grafana") as client:
         client: ManagedGrafanaClient
 
         list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+        list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
         list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
     ```
 """
 from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import UserTypeType
 from .type_defs import (
     ListPermissionsResponseTypeDef,
+    ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
-__all__ = ("ListPermissionsPaginator", "ListWorkspacesPaginator")
-
+__all__ = ("ListPermissionsPaginator", "ListVersionsPaginator", "ListWorkspacesPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListPermissionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listpermissionspaginator)
     """
 
     def paginate(
@@ -63,14 +63,27 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listpermissionspaginator)
         """
 
+class ListVersionsPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listversionspaginator)
+    """
+
+    def paginate(
+        self, *, workspaceId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListVersionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listversionspaginator)
+        """
 
 class ListWorkspacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listworkspacespaginator)
     """
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/paginator.pyi` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/paginator.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,47 +7,53 @@
 
     ```python
     from aiobotocore.session import get_session
 
     from types_aiobotocore_grafana.client import ManagedGrafanaClient
     from types_aiobotocore_grafana.paginator import (
         ListPermissionsPaginator,
+        ListVersionsPaginator,
         ListWorkspacesPaginator,
     )
 
     session = get_session()
     with session.create_client("grafana") as client:
         client: ManagedGrafanaClient
 
         list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+        list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
         list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
     ```
 """
 from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import UserTypeType
 from .type_defs import (
     ListPermissionsResponseTypeDef,
+    ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
-__all__ = ("ListPermissionsPaginator", "ListWorkspacesPaginator")
+__all__ = ("ListPermissionsPaginator", "ListVersionsPaginator", "ListWorkspacesPaginator")
+
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListPermissionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listpermissionspaginator)
     """
 
     def paginate(
@@ -60,14 +66,30 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listpermissionspaginator)
         """
 
+
+class ListVersionsPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listversionspaginator)
+    """
+
+    def paginate(
+        self, *, workspaceId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListVersionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listversionspaginator)
+        """
+
+
 class ListWorkspacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/paginators/#listworkspacespaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/type_defs.py` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,29 +53,32 @@
     "DescribeWorkspaceConfigurationRequestRequestTypeDef",
     "DescribeWorkspaceRequestRequestTypeDef",
     "DisassociateLicenseRequestRequestTypeDef",
     "IdpMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListVersionsRequestRequestTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "UserTypeDef",
     "RoleValuesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
     "CreateWorkspaceApiKeyResponseTypeDef",
     "DeleteWorkspaceApiKeyResponseTypeDef",
     "DescribeWorkspaceConfigurationResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ListVersionsResponseTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
     "WorkspaceDescriptionTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
+    "ListVersionsRequestListVersionsPaginateTypeDef",
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     "PermissionEntryTypeDef",
     "UpdateInstructionTypeDef",
     "SamlConfigurationTypeDef",
     "ListWorkspacesResponseTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
@@ -272,14 +275,24 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListVersionsRequestRequestTypeDef = TypedDict(
+    "ListVersionsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "workspaceId": str,
+    },
+    total=False,
+)
+
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -314,21 +327,36 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateWorkspaceConfigurationRequestRequestTypeDef",
+_RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "configuration": str,
         "workspaceId": str,
     },
 )
+_OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef",
+    {
+        "grafanaVersion": str,
+    },
+    total=False,
+)
+
+
+class UpdateWorkspaceConfigurationRequestRequestTypeDef(
+    _RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef,
+    _OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef,
+):
+    pass
+
 
 CreateWorkspaceApiKeyResponseTypeDef = TypedDict(
     "CreateWorkspaceApiKeyResponseTypeDef",
     {
         "key": str,
         "keyName": str,
         "workspaceId": str,
@@ -345,26 +373,36 @@
     },
 )
 
 DescribeWorkspaceConfigurationResponseTypeDef = TypedDict(
     "DescribeWorkspaceConfigurationResponseTypeDef",
     {
         "configuration": str,
+        "grafanaVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "grafanaVersions": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredWorkspaceSummaryTypeDef = TypedDict(
     "_RequiredWorkspaceSummaryTypeDef",
     {
         "authentication": AuthenticationSummaryTypeDef,
         "created": datetime,
         "endpoint": str,
         "grafanaVersion": str,
@@ -523,14 +561,23 @@
 class ListPermissionsRequestListPermissionsPaginateTypeDef(
     _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
     _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
 ):
     pass
 
 
+ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
+    "ListVersionsRequestListVersionsPaginateTypeDef",
+    {
+        "workspaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListWorkspacesRequestListWorkspacesPaginateTypeDef = TypedDict(
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana/type_defs.pyi` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -52,29 +52,32 @@
     "DescribeWorkspaceConfigurationRequestRequestTypeDef",
     "DescribeWorkspaceRequestRequestTypeDef",
     "DisassociateLicenseRequestRequestTypeDef",
     "IdpMetadataTypeDef",
     "PaginatorConfigTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListVersionsRequestRequestTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "UserTypeDef",
     "RoleValuesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
     "CreateWorkspaceApiKeyResponseTypeDef",
     "DeleteWorkspaceApiKeyResponseTypeDef",
     "DescribeWorkspaceConfigurationResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ListVersionsResponseTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
     "WorkspaceDescriptionTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
+    "ListVersionsRequestListVersionsPaginateTypeDef",
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     "PermissionEntryTypeDef",
     "UpdateInstructionTypeDef",
     "SamlConfigurationTypeDef",
     "ListWorkspacesResponseTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
@@ -267,14 +270,24 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListVersionsRequestRequestTypeDef = TypedDict(
+    "ListVersionsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "workspaceId": str,
+    },
+    total=False,
+)
+
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -309,21 +322,34 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateWorkspaceConfigurationRequestRequestTypeDef",
+_RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "configuration": str,
         "workspaceId": str,
     },
 )
+_OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef",
+    {
+        "grafanaVersion": str,
+    },
+    total=False,
+)
+
+class UpdateWorkspaceConfigurationRequestRequestTypeDef(
+    _RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef,
+    _OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef,
+):
+    pass
 
 CreateWorkspaceApiKeyResponseTypeDef = TypedDict(
     "CreateWorkspaceApiKeyResponseTypeDef",
     {
         "key": str,
         "keyName": str,
         "workspaceId": str,
@@ -340,26 +366,36 @@
     },
 )
 
 DescribeWorkspaceConfigurationResponseTypeDef = TypedDict(
     "DescribeWorkspaceConfigurationResponseTypeDef",
     {
         "configuration": str,
+        "grafanaVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "grafanaVersions": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredWorkspaceSummaryTypeDef = TypedDict(
     "_RequiredWorkspaceSummaryTypeDef",
     {
         "authentication": AuthenticationSummaryTypeDef,
         "created": datetime,
         "endpoint": str,
         "grafanaVersion": str,
@@ -508,14 +544,23 @@
 
 class ListPermissionsRequestListPermissionsPaginateTypeDef(
     _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
     _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
 ):
     pass
 
+ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
+    "ListVersionsRequestListVersionsPaginateTypeDef",
+    {
+        "workspaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListWorkspacesRequestListWorkspacesPaginateTypeDef = TypedDict(
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana.egg-info/PKG-INFO` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-grafana
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ManagedGrafana 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ManagedGrafana 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-grafana.svg?color=blue)](https://pypi.org/project/types-aiobotocore-grafana)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-grafana)](https://pepy.tech/project/types-aiobotocore-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ManagedGrafana 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[aiobotocore.ManagedGrafana 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -271,23 +271,28 @@
 `types_aiobotocore_grafana.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from aiobotocore.session import get_session
 
 from types_aiobotocore_grafana import ManagedGrafanaClient
-from types_aiobotocore_grafana.paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from types_aiobotocore_grafana.paginator import (
+    ListPermissionsPaginator,
+    ListVersionsPaginator,
+    ListWorkspacesPaginator,
+)
 
 session = get_session()
 async with session.create_client("grafana") as client:
     client: ManagedGrafanaClient
 
     # Explicit type annotations are optional here
     # Types should be correctly discovered by mypy and IDEs
     list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+    list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
     list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
 ```
 
 <a id="literals"></a>
 
 ### Literals
```

### Comparing `types-aiobotocore-grafana-2.5.2.post3/types_aiobotocore_grafana.egg-info/SOURCES.txt` & `types-aiobotocore-grafana-2.5.4/types_aiobotocore_grafana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

