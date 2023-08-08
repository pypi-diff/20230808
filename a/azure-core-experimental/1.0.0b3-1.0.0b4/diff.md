# Comparing `tmp/azure-core-experimental-1.0.0b3.zip` & `tmp/azure-core-experimental-1.0.0b4.zip`

## zipinfo {}

```diff
@@ -1,43 +1,43 @@
-Zip file size: 29083 bytes, number of entries: 41
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/samples/
--rw-rw-r--  2.0 unx      278 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/MANIFEST.in
--rw-rw-r--  2.0 unx       98 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/pyproject.toml
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/LICENSE
--rw-rw-r--  2.0 unx     2311 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/setup.py
--rw-rw-r--  2.0 unx      512 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/CHANGELOG.md
--rw-rw-r--  2.0 unx     3000 b- defN 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/PKG-INFO
--rw-rw-r--  2.0 unx     1585 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/README.md
--rw-rw-r--  2.0 unx       38 b- defN 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/setup.cfg
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/azure/core/
--rw-rw-r--  2.0 unx       81 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/azure/core/experimental/
--rw-rw-r--  2.0 unx       81 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/azure/core/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/azure/core/experimental/transport/
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/azure/core/experimental/py.typed
--rw-rw-r--  2.0 unx      172 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/azure/core/experimental/_version.py
--rw-rw-r--  2.0 unx     1357 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/azure/core/experimental/__init__.py
--rw-rw-r--  2.0 unx     5621 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/azure/core/experimental/transport/_httpx_async.py
--rw-rw-r--  2.0 unx     6433 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/azure/core/experimental/transport/_pyodide.py
--rw-rw-r--  2.0 unx     6078 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/azure/core/experimental/transport/_httpx.py
--rw-rw-r--  2.0 unx     2430 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/azure/core/experimental/transport/__init__.py
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx      982 b- defN 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx     3000 b- defN 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        6 b- defN 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/top_level.txt
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/tests/async_tests/
--rw-rw-r--  2.0 unx     7088 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/tests/test_pyodide_transport.py
--rw-rw-r--  2.0 unx     1907 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/tests/test_httpx_transport.py
--rw-rw-r--  2.0 unx     2061 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/tests/async_tests/test_httpx_transport_async.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/samples/pyodide_integration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-10 02:17 azure-core-experimental-1.0.0b3/samples/httpx_integration/
--rw-rw-r--  2.0 unx      855 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/samples/pyodide_integration/async_testing.py
--rw-rw-r--  2.0 unx     5331 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/samples/pyodide_integration/browser.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/samples/httpx_integration/httpx_transport_sample.py
--rw-rw-r--  2.0 unx     1826 b- defN 23-Jul-10 02:16 azure-core-experimental-1.0.0b3/samples/httpx_integration/httpx_transport_sample_async.py
-41 files, 55275 bytes uncompressed, 20989 bytes compressed:  62.0%
+Zip file size: 30787 bytes, number of entries: 41
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/azure/
+-rw-rw-r--  2.0 unx       98 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/pyproject.toml
+-rw-rw-r--  2.0 unx     3201 b- defN 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/PKG-INFO
+-rw-rw-r--  2.0 unx     2311 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/setup.py
+-rw-rw-r--  2.0 unx      278 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/MANIFEST.in
+-rw-rw-r--  2.0 unx      713 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/CHANGELOG.md
+-rw-rw-r--  2.0 unx     1585 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/README.md
+-rw-rw-r--  2.0 unx       38 b- defN 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/setup.cfg
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/LICENSE
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/tests/async_tests/
+-rw-rw-r--  2.0 unx     7088 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/tests/test_pyodide_transport.py
+-rw-rw-r--  2.0 unx     1907 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/tests/test_httpx_transport.py
+-rw-rw-r--  2.0 unx     2061 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/tests/async_tests/test_httpx_transport_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/samples/pyodide_integration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/samples/httpx_integration/
+-rw-rw-r--  2.0 unx      855 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/samples/pyodide_integration/async_testing.py
+-rw-rw-r--  2.0 unx     5331 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/samples/pyodide_integration/browser.py
+-rw-rw-r--  2.0 unx     1823 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/samples/httpx_integration/httpx_transport_sample_async.py
+-rw-rw-r--  2.0 unx     1457 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/samples/httpx_integration/httpx_transport_sample.py
+-rw-rw-r--  2.0 unx     3201 b- defN 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        6 b- defN 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx       26 b- defN 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/requires.txt
+-rw-rw-r--  2.0 unx      982 b- defN 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        1 b- defN 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/dependency_links.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/azure/core/
+-rw-rw-r--  2.0 unx       81 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/azure/core/experimental/
+-rw-rw-r--  2.0 unx       81 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/azure/core/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 20:25 azure-core-experimental-1.0.0b4/azure/core/experimental/transport/
+-rw-rw-r--  2.0 unx      172 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/azure/core/experimental/_version.py
+-rw-rw-r--  2.0 unx     1357 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/azure/core/experimental/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/azure/core/experimental/py.typed
+-rw-rw-r--  2.0 unx     2478 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/azure/core/experimental/transport/__init__.py
+-rw-rw-r--  2.0 unx     8421 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/azure/core/experimental/transport/_httpx.py
+-rw-rw-r--  2.0 unx     7052 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/azure/core/experimental/transport/_pyodide.py
+-rw-rw-r--  2.0 unx     8180 b- defN 23-Aug-07 20:24 azure-core-experimental-1.0.0b4/azure/core/experimental/transport/_httpx_async.py
+41 files, 61858 bytes uncompressed, 22693 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,124 +1,124 @@
-Filename: azure-core-experimental-1.0.0b3/
+Filename: azure-core-experimental-1.0.0b4/
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/
+Filename: azure-core-experimental-1.0.0b4/tests/
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/
+Filename: azure-core-experimental-1.0.0b4/samples/
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/tests/
+Filename: azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/samples/
+Filename: azure-core-experimental-1.0.0b4/azure/
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/MANIFEST.in
+Filename: azure-core-experimental-1.0.0b4/pyproject.toml
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/pyproject.toml
+Filename: azure-core-experimental-1.0.0b4/PKG-INFO
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/LICENSE
+Filename: azure-core-experimental-1.0.0b4/setup.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/setup.py
+Filename: azure-core-experimental-1.0.0b4/MANIFEST.in
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/CHANGELOG.md
+Filename: azure-core-experimental-1.0.0b4/CHANGELOG.md
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/PKG-INFO
+Filename: azure-core-experimental-1.0.0b4/README.md
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/README.md
+Filename: azure-core-experimental-1.0.0b4/setup.cfg
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/setup.cfg
+Filename: azure-core-experimental-1.0.0b4/LICENSE
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/core/
+Filename: azure-core-experimental-1.0.0b4/tests/async_tests/
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/__init__.py
+Filename: azure-core-experimental-1.0.0b4/tests/test_pyodide_transport.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/core/experimental/
+Filename: azure-core-experimental-1.0.0b4/tests/test_httpx_transport.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/core/__init__.py
+Filename: azure-core-experimental-1.0.0b4/tests/async_tests/test_httpx_transport_async.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/core/experimental/transport/
+Filename: azure-core-experimental-1.0.0b4/samples/pyodide_integration/
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/core/experimental/py.typed
+Filename: azure-core-experimental-1.0.0b4/samples/httpx_integration/
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/core/experimental/_version.py
+Filename: azure-core-experimental-1.0.0b4/samples/pyodide_integration/async_testing.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/core/experimental/__init__.py
+Filename: azure-core-experimental-1.0.0b4/samples/pyodide_integration/browser.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/core/experimental/transport/_httpx_async.py
+Filename: azure-core-experimental-1.0.0b4/samples/httpx_integration/httpx_transport_sample_async.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/core/experimental/transport/_pyodide.py
+Filename: azure-core-experimental-1.0.0b4/samples/httpx_integration/httpx_transport_sample.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/core/experimental/transport/_httpx.py
+Filename: azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure/core/experimental/transport/__init__.py
+Filename: azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/not-zip-safe
+Filename: azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/requires.txt
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/requires.txt
+Filename: azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/dependency_links.txt
+Filename: azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/SOURCES.txt
+Filename: azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/PKG-INFO
+Filename: azure-core-experimental-1.0.0b4/azure/core/
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/top_level.txt
+Filename: azure-core-experimental-1.0.0b4/azure/__init__.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/tests/async_tests/
+Filename: azure-core-experimental-1.0.0b4/azure/core/experimental/
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/tests/test_pyodide_transport.py
+Filename: azure-core-experimental-1.0.0b4/azure/core/__init__.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/tests/test_httpx_transport.py
+Filename: azure-core-experimental-1.0.0b4/azure/core/experimental/transport/
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/tests/async_tests/test_httpx_transport_async.py
+Filename: azure-core-experimental-1.0.0b4/azure/core/experimental/_version.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/samples/pyodide_integration/
+Filename: azure-core-experimental-1.0.0b4/azure/core/experimental/__init__.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/samples/httpx_integration/
+Filename: azure-core-experimental-1.0.0b4/azure/core/experimental/py.typed
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/samples/pyodide_integration/async_testing.py
+Filename: azure-core-experimental-1.0.0b4/azure/core/experimental/transport/__init__.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/samples/pyodide_integration/browser.py
+Filename: azure-core-experimental-1.0.0b4/azure/core/experimental/transport/_httpx.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/samples/httpx_integration/httpx_transport_sample.py
+Filename: azure-core-experimental-1.0.0b4/azure/core/experimental/transport/_pyodide.py
 Comment: 
 
-Filename: azure-core-experimental-1.0.0b3/samples/httpx_integration/httpx_transport_sample_async.py
+Filename: azure-core-experimental-1.0.0b4/azure/core/experimental/transport/_httpx_async.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-core-experimental-1.0.0b3/LICENSE` & `azure-core-experimental-1.0.0b4/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-core-experimental-1.0.0b3/setup.py` & `azure-core-experimental-1.0.0b4/setup.py`

 * *Files identical despite different names*

## Comparing `azure-core-experimental-1.0.0b3/PKG-INFO` & `azure-core-experimental-1.0.0b4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-core-experimental
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Microsoft Azure Core Experimental Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core-experimental
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -45,14 +45,21 @@
 When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
 
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 
 # Release History
 
+## 1.0.0b4 (2023-08-03)
+
+### Bugs Fixed
+
+- Create new httpx client when used without "with" ([#31362](https://github.com/Azure/azure-sdk-for-python/pull/31370))
+- Fix httpx sample with right API name
+
 ## 1.0.0b3 (2023-07-06)
 
 ### Bug Fixes
 
 - Update httpx transport to handle timeout and connection verify kwargs from `azure.core.pipeline.transport.HttpRequest`.
 - Add a read override for `read` for clients using `azure.core.rest.HttpResponse` to get the response body.
```

## Comparing `azure-core-experimental-1.0.0b3/README.md` & `azure-core-experimental-1.0.0b4/README.md`

 * *Files identical despite different names*

## Comparing `azure-core-experimental-1.0.0b3/azure/core/experimental/__init__.py` & `azure-core-experimental-1.0.0b4/azure/core/experimental/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-core-experimental-1.0.0b3/azure/core/experimental/transport/_httpx_async.py` & `azure-core-experimental-1.0.0b4/azure/core/experimental/transport/_httpx_async.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,65 +19,95 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
-from typing import ContextManager, Optional, Any, AsyncIterator
+from typing import Any, AsyncIterator, ContextManager, Optional, Union
 
 import httpx
+from azure.core.configuration import ConnectionConfiguration
+from azure.core.exceptions import DecodeError, ServiceRequestError, ServiceResponseError
 from azure.core.pipeline import Pipeline
-
-from azure.core.exceptions import ServiceRequestError, ServiceResponseError
 from azure.core.pipeline.transport import AsyncHttpTransport
+from azure.core.pipeline.transport import HttpRequest as LegacyHttpRequest
 from azure.core.rest import HttpRequest
 from azure.core.rest._http_response_impl_async import AsyncHttpResponseImpl
 
 
 class AsyncHttpXTransportResponse(AsyncHttpResponseImpl):
+    """Async HttpX response implementation.
+
+    :param request: The request sent to the server
+    :type request: ~azure.core.rest.HTTPRequest or LegacyHTTPRequest
+    :param httpx.Response httpx_response: The response object returned from HttpX library
+    :param ContextManager stream_contextmanager: The context manager to stream response data.
+    """
+
     def __init__(
-        self, request: HttpRequest, httpx_response: httpx.Response, stream_contextmanager: Optional[ContextManager]
+        self,
+        request: Union[HttpRequest, LegacyHttpRequest],
+        httpx_response: httpx.Response,
+        stream_contextmanager: Optional[ContextManager],
     ) -> None:
         super().__init__(
             request=request,
             internal_response=httpx_response,
             status_code=httpx_response.status_code,
             headers=httpx_response.headers,
             reason=httpx_response.reason_phrase,
             content_type=httpx_response.headers.get("content-type"),
             stream_download_generator=stream_contextmanager,
         )
 
     def body(self) -> bytes:
+        """Return the whole body as bytes.
+
+        :return: The whole body as bytes.
+        :rtype: bytes
+        """
         return self.internal_response.content
 
     def stream_download(self, pipeline: Pipeline, **kwargs: Any) -> AsyncIterator[bytes]:
+        """Generator for streaming response data.
+
+        :param pipeline: The pipeline object
+        :type pipeline: ~azure.core.pipeline.Pipeline
+        :keyword bool decompress: If True which is default, will attempt to decode the body based
+            on the *content-encoding* header.
+        :return: An iterator for streaming response data.
+        :rtype: AsyncIterator[bytes]
+        """
         return AsyncHttpXStreamDownloadGenerator(pipeline, self, **kwargs)
 
     async def load_body(self) -> None:
         self._content = await self.internal_response.read()
 
 
 # pylint: disable=unused-argument
 class AsyncHttpXStreamDownloadGenerator(AsyncIterator):
     """Generator for streaming response data.
 
     :param pipeline: The pipeline object
+    :type pipeline: ~azure.core.pipeline.Pipeline
     :param response: The response object.
+    :type response: AsyncHttpXTransportResponse
     :keyword bool decompress: If True which is default, will attempt to decode the body based
         on the *content-encoding* header.
     """
 
-    def __init__(self, pipeline: Pipeline, response: AsyncHttpXTransportResponse, *_, **kwargs) -> None:
+    def __init__(
+        self, pipeline: Pipeline, response: AsyncHttpXTransportResponse, *, decompress: bool = True, **kwargs
+    ) -> None:
         self.pipeline = pipeline
         self.response = response
-        decompress = kwargs.pop("decompress", True)
+        should_decompress = decompress
 
-        if decompress:
+        if should_decompress:
             self.iter_content_func = self.response.internal_response.aiter_bytes()
         else:
             self.iter_content_func = self.response.internal_response.aiter_raw()
 
     async def __len__(self) -> int:
         return self.response.internal_response.headers["content-length"]
 
@@ -86,42 +116,71 @@
 
     async def __anext__(self):
         try:
             return await self.iter_content_func.__anext__()
         except StopAsyncIteration:
             self.response.internal_response.close()
             raise
+        except httpx.DecodingError as ex:
+            if len(ex.args) > 1:
+                raise DecodeError(ex.args[0]) from ex
+            raise DecodeError("Failed to decode.") from ex
 
 
 class AsyncHttpXTransport(AsyncHttpTransport):
     """Implements a basic async httpx HTTP sender
 
     :keyword httpx.AsyncClient client: HTTPX client to use instead of the default one
+    :keyword bool client_owner: Decide if the client provided by user is owned by this transport. Default to True.
+    :keyword bool use_env_settings: Uses proxy settings from environment. Defaults to True.
     """
 
-    def __init__(self, **kwargs: Any) -> None:
-        self.client = kwargs.get("client", None)
+    def __init__(
+        self,
+        *,
+        client: Optional[httpx.AsyncClient] = None,
+        client_owner: bool = True,
+        use_env_settings: bool = True,
+        **kwargs: Any
+    ) -> None:
+        self.client = client
+        self.connection_config = ConnectionConfiguration(**kwargs)
+        self._client_owner = client_owner
+        self._use_env_settings = use_env_settings
 
     async def open(self) -> None:
         if self.client is None:
-            self.client = httpx.AsyncClient()
+            self.client = httpx.AsyncClient(
+                trust_env=self._use_env_settings,
+                verify=self.connection_config.verify,
+                cert=self.connection_config.cert,
+            )
 
     async def close(self) -> None:
-        if self.client:
+        if self._client_owner and self.client:
             await self.client.aclose()
             self.client = None
 
     async def __aenter__(self) -> "AsyncHttpXTransport":
         await self.open()
         return self
 
     async def __aexit__(self, *args) -> None:
         await self.close()
 
-    async def send(self, request: HttpRequest, **kwargs) -> AsyncHttpXTransportResponse:
+    async def send(self, request: Union[HttpRequest, LegacyHttpRequest], **kwargs) -> AsyncHttpXTransportResponse:
+        """Send the request using this HTTP sender.
+
+        :param request: The request object to be sent.
+        :type request: ~azure.core.rest.HttpRequest or LegacyHttpRequest
+        :keyword bool stream: Whether to stream the response. Defaults to False.
+        :return: The response object.
+        :rtype: ~azure.core.experimental.transport.AsyncHttpXTransportResponse
+        """
+        await self.open()
         stream_response = kwargs.pop("stream", False)
         parameters = {
             "method": request.method,
             "url": request.url,
             "headers": request.headers.items(),
             "data": request.data,
             "content": request.content,
@@ -137,12 +196,12 @@
                 response = await self.client.send(req, stream=stream_response)
             else:
                 response = await self.client.request(**parameters)
         except (
             httpx.ReadTimeout,
             httpx.ProtocolError,
         ) as err:
-            raise ServiceResponseError(err, error=err)
+            raise ServiceResponseError(err, error=err) from err
         except httpx.RequestError as err:
-            raise ServiceRequestError(err, error=err)
+            raise ServiceRequestError(err, error=err) from err
 
         return AsyncHttpXTransportResponse(request, response, stream_contextmanager=stream_ctx)
```

## Comparing `azure-core-experimental-1.0.0b3/azure/core/experimental/transport/_pyodide.py` & `azure-core-experimental-1.0.0b4/azure/core/experimental/transport/_pyodide.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,50 +25,69 @@
 # --------------------------------------------------------------------------
 
 from collections.abc import AsyncIterator
 from io import BytesIO
 
 import js  # pylint: disable=import-error
 from pyodide import JsException  # pylint: disable=import-error
-from pyodide.http import pyfetch  # pylint: disable=import-error
+from pyodide.http import pyfetch, FetchResponse  # pylint: disable=import-error
 
 from azure.core.exceptions import HttpResponseError
 from azure.core.pipeline import Pipeline
 from azure.core.utils import CaseInsensitiveDict
 
 from azure.core.rest._http_response_impl_async import AsyncHttpResponseImpl
-from azure.core.pipeline.transport import HttpRequest, AsyncioRequestsTransport
+from azure.core.pipeline.transport import (  # pylint: disable=non-abstract-transport-import, no-name-in-module
+    HttpRequest,
+    AsyncioRequestsTransport,
+)
 
 
 class PyodideTransportResponse(AsyncHttpResponseImpl):
     """Async response object for the `PyodideTransport`."""
 
-    def _js_stream(self):
-        """So we get a fresh stream every time."""
+    def _js_stream(self) -> FetchResponse:
+        """So we get a fresh stream every time.
+
+        :return: The stream stream
+        :rtype: ~pyodide.http.FetchResponse
+        """
         return self._internal_response.clone().js_response.body
 
     async def close(self) -> None:
         """We don't actually have control over closing connections in the browser, so we just pretend
         to close.
+
+        :return: None
+        :rtype: None
         """
         self._is_closed = True
 
     def body(self) -> bytes:
-        """The body is just the content."""
+        """The body is just the content.
+
+        :return: The body of the response.
+        :rtype: bytes
+        """
         return self.content
 
     async def load_body(self) -> None:
         """Backcompat"""
         if self._content is None:
             self._content = await self._internal_response.clone().bytes()
 
 
 class PyodideStreamDownloadGenerator(AsyncIterator):
     """Simple stream download generator that returns the contents of
     a request.
+
+    :param pipeline: The pipeline object
+    :type pipeline: ~azure.core.pipeline.Pipeline
+    :param response: The response object
+    :type response: ~azure.core.experimental.transport.PyodideTransportResponse
     """
 
     # pylint: disable=unused-argument
     def __init__(self, pipeline: Pipeline, response: PyodideTransportResponse, *_, **kwargs):
         self._block_size = response._block_size
         self.response = response
         # use this to efficiently store bytes.
@@ -81,15 +100,19 @@
         self._closed = False
         # We cannot control how many bytes we get from `response.reader`. `self._buffer_left`
         # indicates how many unread bytes there are in `self.stream`
         self._buffer_left = 0
         self.done = False
 
     async def __anext__(self) -> bytes:
-        """Get the next block of bytes."""
+        """Get the next block of bytes.
+
+        :return: The next block of bytes.
+        :rtype: bytes
+        """
         if self._closed:
             raise StopAsyncIteration()
 
         # remember the initial stream position
         start_pos = self._stream.tell()
         # move stream position to the end
         self._stream.read()
@@ -136,15 +159,15 @@
             "allow_redirects": False,
             **kwargs,
         }
 
         try:
             response = await pyfetch(endpoint, **init)
         except JsException as error:
-            raise HttpResponseError(error, error=error)
+            raise HttpResponseError(error, error=error) from error
 
         headers = CaseInsensitiveDict(response.js_response.headers)
         transport_response = PyodideTransportResponse(
             request=request,
             internal_response=response,
             block_size=self.connection_config.data_block_size,
             status_code=response.status,
```

## Comparing `azure-core-experimental-1.0.0b3/azure/core/experimental/transport/_httpx.py` & `azure-core-experimental-1.0.0b4/azure/core/experimental/transport/_httpx.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,115 +19,177 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
-from typing import Any, ContextManager, Iterator, Optional
+from typing import Any, ContextManager, Iterator, Optional, Union
 
 import httpx
+from azure.core.configuration import ConnectionConfiguration
+from azure.core.exceptions import DecodeError, ServiceRequestError, ServiceResponseError
 from azure.core.pipeline import Pipeline
-
-from azure.core.exceptions import ServiceRequestError, ServiceResponseError
 from azure.core.pipeline.transport import HttpTransport
 from azure.core.rest import HttpRequest
 from azure.core.rest._http_response_impl import HttpResponseImpl
-from azure.core.configuration import ConnectionConfiguration
+from azure.core.pipeline.transport import HttpRequest as LegacyHttpRequest
 
 
 class HttpXTransportResponse(HttpResponseImpl):
+    """HttpX response implementation.
+
+    :param request: The request sent to the server
+    :type request: ~azure.core.rest.HTTPRequest or LegacyHTTPRequest
+    :param httpx.Response httpx_response: The response object returned from the HttpX library
+    :param ContextManager stream_contextmanager: The context manager to stream response data.
+    """
+
     def __init__(
-        self, request: HttpRequest, httpx_response: httpx.Response, stream_contextmanager: Optional[ContextManager]
+        self,
+        request: Union[HttpRequest, LegacyHttpRequest],
+        httpx_response: httpx.Response,
+        stream_contextmanager: Optional[ContextManager],
     ) -> None:
         super().__init__(
             request=request,
             internal_response=httpx_response,
             status_code=httpx_response.status_code,
             headers=httpx_response.headers,
             reason=httpx_response.reason_phrase,
             content_type=httpx_response.headers.get("content-type"),
             stream_download_generator=stream_contextmanager,
         )
 
     def read(self) -> bytes:
+        """Read the response's bytes.
+
+        :return: The response's bytes.
+        :rtype: bytes
+        """
         if self._content is None:
             self._content = self.internal_response.read()
         return self.content
 
     def body(self) -> bytes:
+        """Get the body of the response.
+
+        :return: The response's bytes.
+        :rtype: bytes
+        """
         return self.internal_response.content
 
     def stream_download(self, pipeline: Pipeline, **kwargs) -> Iterator[bytes]:
+        """Generator for streaming response data.
+
+        :param pipeline: The pipeline object
+        :type pipeline: ~azure.core.pipeline.Pipeline
+        :keyword bool decompress: If True which is default, will attempt to decode the body based
+            on the *content-encoding* header.
+        :return: An iterator for streaming response data.
+        :rtype: Iterator[bytes]
+        """
         return HttpXStreamDownloadGenerator(pipeline, self, **kwargs)
 
 
 # pylint: disable=unused-argument
 class HttpXStreamDownloadGenerator:
     """Generator for streaming response data.
 
     :param pipeline: The pipeline object
+    :type pipeline: ~azure.core.pipeline.Pipeline
     :param response: The response object.
+    :type response: HttpXTransportResponse
     :keyword bool decompress: If True which is default, will attempt to decode the body based
         on the *content-encoding* header.
     """
 
-    def __init__(self, pipeline: Pipeline, response: HttpXTransportResponse, **kwargs) -> None:
+    def __init__(
+        self, pipeline: Pipeline, response: HttpXTransportResponse, *, decompress: bool = True, **kwargs
+    ) -> None:
         self.pipeline = pipeline
         self.response = response
-        decompress = kwargs.pop("decompress", True)
+        should_decompress = decompress
 
-        if decompress:
+        if should_decompress:
             self.iter_content_func = self.response.internal_response.iter_bytes()
         else:
             self.iter_content_func = self.response.internal_response.iter_raw()
 
     def __iter__(self) -> "HttpXStreamDownloadGenerator":
         return self
 
     def __next__(self):
         try:
             return next(self.iter_content_func)
         except StopIteration:
             self.response.stream_contextmanager.__exit__(None, None, None)
             raise
+        except httpx.DecodingError as ex:
+            if len(ex.args) > 0:
+                raise DecodeError(ex.args[0]) from ex
+            raise DecodeError("Failed to decode.") from ex
 
 
 class HttpXTransport(HttpTransport):
     """Implements a basic httpx HTTP sender
 
     :keyword httpx.Client client: HTTPX client to use instead of the default one
+    :keyword bool client_owner: Decide if the client provided by user is owned by this transport. Default to True.
+    :keyword bool use_env_settings: Uses proxy settings from environment. Defaults to True.
     """
 
-    def __init__(self, *, client: Optional[httpx.Client] = None, **kwargs: Any) -> None:
+    def __init__(
+        self,
+        *,
+        client: Optional[httpx.Client] = None,
+        client_owner: bool = True,
+        use_env_settings: bool = True,
+        **kwargs: Any
+    ) -> None:
         self.client = client
         self.connection_config = ConnectionConfiguration(**kwargs)
-        self._use_env_settings = kwargs.pop("use_env_settings", True)
+        self._client_owner = client_owner
+        self._use_env_settings = use_env_settings
 
     def open(self) -> None:
         if self.client is None:
             self.client = httpx.Client(
                 trust_env=self._use_env_settings,
                 verify=self.connection_config.verify,
                 cert=self.connection_config.cert,
             )
 
     def close(self) -> None:
-        if self.client:
+        """Close the session.
+
+        :return: None
+        :rtype: None
+        """
+        if self._client_owner and self.client:
             self.client.close()
             self.client = None
 
     def __enter__(self) -> "HttpXTransport":
         self.open()
         return self
 
     def __exit__(self, *args) -> None:
         self.close()
 
-    def send(self, request: HttpRequest, **kwargs) -> HttpXTransportResponse:
+    def send(self, request: Union[HttpRequest, LegacyHttpRequest], **kwargs) -> HttpXTransportResponse:
+        """Send a request and get back a response.
+
+        :param request: The request object to be sent.
+        :type request: ~azure.core.rest.HTTPRequest or LegacyHTTPRequest
+        :keyword bool stream: Whether to stream the response. Defaults to False.
+        :return: An HTTPResponse object.
+        :rtype: ~azure.core.experimental.transport.HttpXTransportResponse
+        """
+        self.open()
         stream_response = kwargs.pop("stream", False)
         timeout = kwargs.pop("connection_timeout", self.connection_config.timeout)
         # not needed here as its already handled during init
         kwargs.pop("connection_verify", None)
         parameters = {
             "method": request.method,
             "url": request.url,
@@ -149,12 +211,12 @@
                     response = stream_ctx.__enter__()
             else:
                 response = self.client.request(**parameters)
         except (
             httpx.ReadTimeout,
             httpx.ProtocolError,
         ) as err:
-            raise ServiceResponseError(err, error=err)
+            raise ServiceResponseError(err, error=err) from err
         except httpx.RequestError as err:
-            raise ServiceRequestError(err, error=err)
+            raise ServiceRequestError(err, error=err) from err
 
         return HttpXTransportResponse(request, response, stream_contextmanager=stream_ctx)
```

## Comparing `azure-core-experimental-1.0.0b3/azure/core/experimental/transport/__init__.py` & `azure-core-experimental-1.0.0b4/azure/core/experimental/transport/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,25 +39,25 @@
 
     def __getattr__(name):
         if name == "PyodideTransport":
             try:
                 from ._pyodide import PyodideTransport
 
                 return PyodideTransport
-            except ImportError:
-                raise ImportError("pyodide package is not installed")
+            except ImportError as err:
+                raise ImportError("pyodide package is not installed") from err
         if name == "HttpXTransport":
             try:
                 from ._httpx import HttpXTransport
 
                 return HttpXTransport
-            except ImportError:
-                raise ImportError("httpx package is not installed")
+            except ImportError as err:
+                raise ImportError("httpx package is not installed") from err
         if name == "AsyncHttpXTransport":
             try:
                 from ._httpx_async import AsyncHttpXTransport
 
                 return AsyncHttpXTransport
-            except ImportError:
-                raise ImportError("httpx package is not installed")
+            except ImportError as err:
+                raise ImportError("httpx package is not installed") from err
 
         raise AttributeError(f"module 'azure.core.experimental.transport' has no attribute {name}")
```

## Comparing `azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/SOURCES.txt` & `azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `azure-core-experimental-1.0.0b3/azure_core_experimental.egg-info/PKG-INFO` & `azure-core-experimental-1.0.0b4/azure_core_experimental.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-core-experimental
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Microsoft Azure Core Experimental Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core-experimental
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -45,14 +45,21 @@
 When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
 
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 
 # Release History
 
+## 1.0.0b4 (2023-08-03)
+
+### Bugs Fixed
+
+- Create new httpx client when used without "with" ([#31362](https://github.com/Azure/azure-sdk-for-python/pull/31370))
+- Fix httpx sample with right API name
+
 ## 1.0.0b3 (2023-07-06)
 
 ### Bug Fixes
 
 - Update httpx transport to handle timeout and connection verify kwargs from `azure.core.pipeline.transport.HttpRequest`.
 - Add a read override for `read` for clients using `azure.core.rest.HttpResponse` to get the response body.
```

## Comparing `azure-core-experimental-1.0.0b3/tests/test_pyodide_transport.py` & `azure-core-experimental-1.0.0b4/tests/test_pyodide_transport.py`

 * *Files identical despite different names*

## Comparing `azure-core-experimental-1.0.0b3/tests/test_httpx_transport.py` & `azure-core-experimental-1.0.0b4/tests/test_httpx_transport.py`

 * *Files identical despite different names*

## Comparing `azure-core-experimental-1.0.0b3/tests/async_tests/test_httpx_transport_async.py` & `azure-core-experimental-1.0.0b4/tests/async_tests/test_httpx_transport_async.py`

 * *Files identical despite different names*

## Comparing `azure-core-experimental-1.0.0b3/samples/pyodide_integration/async_testing.py` & `azure-core-experimental-1.0.0b4/samples/pyodide_integration/async_testing.py`

 * *Files identical despite different names*

## Comparing `azure-core-experimental-1.0.0b3/samples/pyodide_integration/browser.py` & `azure-core-experimental-1.0.0b4/samples/pyodide_integration/browser.py`

 * *Files identical despite different names*

## Comparing `azure-core-experimental-1.0.0b3/samples/httpx_integration/httpx_transport_sample_async.py` & `azure-core-experimental-1.0.0b4/samples/httpx_integration/httpx_transport_sample_async.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         credential=AzureKeyCredential(key),
         transport=AsyncHttpXTransport(),
     )
 
     document = ["This is an example document."]
 
     async with text_analytics_client:
-        poller = await text_analytics_client.begin_abstractive_summary(document)
+        poller = await text_analytics_client.begin_abstract_summary(document)
         abstractive_summary_results = await poller.result()
         async for result in abstractive_summary_results:
             if result.kind == "AbstractiveSummarization":
                 print("Summaries abstracted:")
                 [print(f"{summary.text}\n") for summary in result.summaries]
             elif result.is_error is True:
                 print("...Is an error with code '{}' and message '{}'".format(result.error.code, result.error.message))
```

