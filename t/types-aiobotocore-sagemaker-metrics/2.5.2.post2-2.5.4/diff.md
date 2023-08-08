# Comparing `tmp/types-aiobotocore-sagemaker-metrics-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-sagemaker-metrics-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-metrics-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-metrics-2.5.4.tar", last modified: Tue Aug  8 01:24:23 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2.tar` & `types-aiobotocore-sagemaker-metrics-2.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.996643 types-aiobotocore-sagemaker-metrics-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12731 2023-08-04 13:59:24.996643 types-aiobotocore-sagemaker-metrics-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11174 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:24.996643 types-aiobotocore-sagemaker-metrics-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2141 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.996643 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      517 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      516 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      981 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4725 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4716 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8417 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8415 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2097 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.996643 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12731 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      904 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       36 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:23.066772 types-aiobotocore-sagemaker-metrics-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-08-08 01:24:23.066772 types-aiobotocore-sagemaker-metrics-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:24:23.066772 types-aiobotocore-sagemaker-metrics-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:23.058772 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 01:20:31.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:24:23.058772 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 01:24:22.000000 types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/LICENSE` & `types-aiobotocore-sagemaker-metrics-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/PKG-INFO` & `types-aiobotocore-sagemaker-metrics-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-metrics
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SageMakerMetrics 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SageMakerMetrics 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-metrics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-metrics)](https://pepy.tech/project/types-aiobotocore-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMakerMetrics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[aiobotocore.SageMakerMetrics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/README.md` & `types-aiobotocore-sagemaker-metrics-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-metrics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-metrics)](https://pepy.tech/project/types-aiobotocore-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMakerMetrics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[aiobotocore.SageMakerMetrics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/setup.py` & `types-aiobotocore-sagemaker-metrics-2.5.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-metrics",
-    version="2.5.2.post2",
+    version="2.5.4",
     packages=["types_aiobotocore_sagemaker_metrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SageMakerMetrics 2.5.2 service generated with"
+        "Type annotations for aiobotocore.SageMakerMetrics 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/__init__.py` & `types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/__init__.pyi` & `types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/client.py` & `types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/client.pyi` & `types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/literals.py` & `types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/literals.pyi` & `types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/type_defs.py` & `types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/type_defs.pyi` & `types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-metrics
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.SageMakerMetrics 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.SageMakerMetrics 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-metrics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-metrics)](https://pepy.tech/project/types-aiobotocore-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMakerMetrics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[aiobotocore.SageMakerMetrics 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-metrics-2.5.4/types_aiobotocore_sagemaker_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

