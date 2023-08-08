# Comparing `tmp/apache-airflow-providers-celery-3.3.0rc1.tar.gz` & `tmp/apache-airflow-providers-celery-3.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-celery-3.3.0rc1.tar", last modified: Sat Jul 29 12:08:10 2023, max compression
+gzip compressed data, was "apache-airflow-providers-celery-3.3.1rc1.tar", last modified: Fri Aug  4 21:40:53 2023, max compression
```

## Comparing `apache-airflow-providers-celery-3.3.0rc1.tar` & `apache-airflow-providers-celery-3.3.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.464499 apache-airflow-providers-celery-3.3.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.3.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.3.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5581 2023-07-29 12:08:10.465122 apache-airflow-providers-celery-3.3.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3911 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.376279 apache-airflow-providers-celery-3.3.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.377486 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.414891 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/
--rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.430149 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/
--rw-r--r--   0 root         (0) root         (0)     1584 2023-07-12 12:42:21.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18336 2023-07-29 09:53:35.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_executor.py
--rw-r--r--   0 root         (0) root         (0)    13011 2023-07-26 06:59:50.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_executor_utils.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-07-29 06:50:08.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_kubernetes_executor.py
--rw-r--r--   0 root         (0) root         (0)     5800 2023-07-26 06:59:50.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/default_celery.py
--rw-r--r--   0 root         (0) root         (0)    16209 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.437531 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2780 2023-06-29 05:49:30.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/celery_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.461789 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5581 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      913 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-celery-3.3.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1958 2023-07-29 12:08:10.466958 apache-airflow-providers-celery-3.3.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1708 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:53.161849 apache-airflow-providers-celery-3.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:40:52.000000 apache-airflow-providers-celery-3.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5581 2023-08-04 21:40:53.162471 apache-airflow-providers-celery-3.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-08-04 21:40:52.000000 apache-airflow-providers-celery-3.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:53.082390 apache-airflow-providers-celery-3.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:53.083643 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:53.114700 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-08-04 21:33:34.000000 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:53.129188 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/executors/
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-07-12 12:42:21.000000 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/executors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18521 2023-08-04 19:44:14.000000 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/executors/celery_executor.py
+-rw-r--r--   0 root         (0) root         (0)    12993 2023-08-04 10:24:22.000000 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/executors/celery_executor_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-07-29 06:50:08.000000 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/executors/celery_kubernetes_executor.py
+-rw-r--r--   0 root         (0) root         (0)     5800 2023-07-26 06:59:50.000000 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/executors/default_celery.py
+-rw-r--r--   0 root         (0) root         (0)    16230 2023-08-04 21:40:52.000000 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:53.134839 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-06-29 05:49:30.000000 apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/sensors/celery_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:53.159269 apache-airflow-providers-celery-3.3.1rc1/apache_airflow_providers_celery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5581 2023-08-04 21:40:53.000000 apache-airflow-providers-celery-3.3.1rc1/apache_airflow_providers_celery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      913 2023-08-04 21:40:53.000000 apache-airflow-providers-celery-3.3.1rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:53.000000 apache-airflow-providers-celery-3.3.1rc1/apache_airflow_providers_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-08-04 21:40:53.000000 apache-airflow-providers-celery-3.3.1rc1/apache_airflow_providers_celery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:53.000000 apache-airflow-providers-celery-3.3.1rc1/apache_airflow_providers_celery.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2023-08-04 21:40:53.000000 apache-airflow-providers-celery-3.3.1rc1/apache_airflow_providers_celery.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:53.000000 apache-airflow-providers-celery-3.3.1rc1/apache_airflow_providers_celery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-celery-3.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-08-04 21:40:53.164372 apache-airflow-providers-celery-3.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-08-04 21:40:51.000000 apache-airflow-providers-celery-3.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-celery-3.3.0rc1/LICENSE` & `apache-airflow-providers-celery-3.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0rc1/MANIFEST.in` & `apache-airflow-providers-celery-3.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0rc1/PKG-INFO` & `apache-airflow-providers-celery-3.3.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-celery
-Version: 3.3.0rc1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-celery package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -67,28 +67,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.3.0rc1``
+Release: ``3.3.1rc1``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``celery`` provider. All classes for this provider package
 are in ``airflow.providers.celery`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -123,8 +123,8 @@
 ======================================================================================================================  ===================
 Dependent package                                                                                                       Extra
 ======================================================================================================================  ===================
 `apache-airflow-providers-cncf-kubernetes <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes>`_  ``cncf.kubernetes``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-celery-3.3.0rc1/README.rst` & `apache-airflow-providers-celery-3.3.1rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.3.0rc1``
+Release: ``3.3.1rc1``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``celery`` provider. All classes for this provider package
 are in ``airflow.providers.celery`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -88,8 +88,8 @@
 ======================================================================================================================  ===================
 Dependent package                                                                                                       Extra
 ======================================================================================================================  ===================
 `apache-airflow-providers-cncf-kubernetes <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes>`_  ``cncf.kubernetes``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/__init__.py` & `apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.3.0"
+__version__ = "3.3.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/__init__.py` & `apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_executor.py` & `apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/executors/celery_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 .. seealso::
     For more information on how the CeleryExecutor works, take a look at the guide:
     :ref:`executor:CeleryExecutor`
 """
 from __future__ import annotations
 
+import argparse
 import logging
 import math
 import operator
 import time
 from collections import Counter
 from concurrent.futures import ProcessPoolExecutor
 from multiprocessing import cpu_count
@@ -260,15 +261,15 @@
 
     def _num_tasks_per_send_process(self, to_send_count: int) -> int:
         """
         How many Celery tasks should each worker process send.
 
         :return: Number of tasks that should be sent per process
         """
-        return max(1, int(math.ceil(1.0 * to_send_count / self._sync_parallelism)))
+        return max(1, math.ceil(to_send_count / self._sync_parallelism))
 
     def _process_tasks(self, task_tuples: list[TaskTuple]) -> None:
         from airflow.providers.celery.executors.celery_executor_utils import execute_command
 
         task_tuples_to_send = [task_tuple[:3] + (execute_command,) for task_tuple in task_tuples]
         first_task = next(t[3] for t in task_tuples_to_send)
 
@@ -476,7 +477,15 @@
                 description=(
                     "Start celery components. Works only when using CeleryExecutor. For more information, "
                     "see https://airflow.apache.org/docs/apache-airflow/stable/executor/celery.html"
                 ),
                 subcommands=CELERY_COMMANDS,
             ),
         ]
+
+
+def _get_parser() -> argparse.ArgumentParser:
+    """This method is used by Sphinx to generate documentation.
+
+    :meta private:
+    """
+    return CeleryExecutor._get_parser()
```

### Comparing `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_executor_utils.py` & `apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/executors/celery_executor_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
             state_info[task_id] = state, info
         return state_info
 
     def _get_many_using_multiprocessing(self, async_results) -> Mapping[str, EventBufferValueType]:
         num_process = min(len(async_results), self._sync_parallelism)
 
         with ProcessPoolExecutor(max_workers=num_process) as sync_pool:
-            chunksize = max(1, math.floor(math.ceil(1.0 * len(async_results) / self._sync_parallelism)))
+            chunksize = max(1, math.ceil(len(async_results) / self._sync_parallelism))
 
             task_id_to_states_and_info = list(
                 sync_pool.map(fetch_celery_task_state, async_results, chunksize=chunksize)
             )
 
             states_and_info_by_task_id: MutableMapping[str, EventBufferValueType] = {}
             for task_id, state_or_exception, info in task_id_to_states_and_info:
```

### Comparing `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_kubernetes_executor.py` & `apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/executors/celery_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/default_celery.py` & `apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/executors/default_celery.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/get_provider_info.py` & `apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-celery",
         "name": "Celery",
         "description": "`Celery <http://www.celeryproject.org/>`__\n",
         "suspended": False,
         "versions": [
+            "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.1.4",
             "2.1.3",
```

### Comparing `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/__init__.py` & `apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/celery_queue.py` & `apache-airflow-providers-celery-3.3.1rc1/airflow/providers/celery/sensors/celery_queue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/PKG-INFO` & `apache-airflow-providers-celery-3.3.1rc1/apache_airflow_providers_celery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-celery
-Version: 3.3.0rc1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-celery package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -67,28 +67,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.3.0rc1``
+Release: ``3.3.1rc1``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``celery`` provider. All classes for this provider package
 are in ``airflow.providers.celery`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -123,8 +123,8 @@
 ======================================================================================================================  ===================
 Dependent package                                                                                                       Extra
 ======================================================================================================================  ===================
 `apache-airflow-providers-cncf-kubernetes <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes>`_  ``cncf.kubernetes``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt` & `apache-airflow-providers-celery-3.3.1rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.3.0rc1/pyproject.toml` & `apache-airflow-providers-celery-3.3.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
     "ignore::DeprecationWarning:flask_sqlalchemy",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
     "ignore::DeprecationWarning:apispec.utils",
 ]
 python_files = [
     "test_*.py",
+    "example_*.py",
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff.isort]
 required-imports = ["from __future__ import annotations"]
```

### Comparing `apache-airflow-providers-celery-3.3.0rc1/setup.cfg` & `apache-airflow-providers-celery-3.3.1rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-celery-3.3.0rc1/setup.py` & `apache-airflow-providers-celery-3.3.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-celery package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.3.0"
+version = "3.3.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-celery setup."""
     setup(
         version=version,
         extras_require={"cncf.kubernetes": ["apache-airflow-providers-cncf-kubernetes>=7.4.0"]},
```

