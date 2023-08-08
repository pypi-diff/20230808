# Comparing `tmp/apache-airflow-providers-asana-2.2.2rc1.tar.gz` & `tmp/apache-airflow-providers-asana-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-asana-2.2.2rc1.tar", last modified: Fri Aug  4 21:40:50 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-asana-3.0.0rc1.tar", last modified: Tue Nov 15 00:14:08 2022, max compression
```

## Comparing `apache-airflow-providers-asana-2.2.2rc1.tar` & `apache-airflow-providers-asana-3.0.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:50.619617 apache-airflow-providers-asana-2.2.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-asana-2.2.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:40:49.000000 apache-airflow-providers-asana-2.2.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-asana-2.2.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4395 2023-08-04 21:40:50.620176 apache-airflow-providers-asana-2.2.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2761 2023-08-04 21:40:49.000000 apache-airflow-providers-asana-2.2.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:50.547583 apache-airflow-providers-asana-2.2.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:50.548749 apache-airflow-providers-asana-2.2.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:50.581446 apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/
--rw-r--r--   0 root         (0) root         (0)     1574 2023-08-04 21:33:34.000000 apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-08-04 21:40:49.000000 apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:50.587638 apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13309 2023-06-29 05:49:30.000000 apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/hooks/asana.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:50.593399 apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5491 2023-06-05 12:50:36.000000 apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/operators/asana_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:50.617004 apache-airflow-providers-asana-2.2.2rc1/apache_airflow_providers_asana.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4395 2023-08-04 21:40:50.000000 apache-airflow-providers-asana-2.2.2rc1/apache_airflow_providers_asana.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      707 2023-08-04 21:40:50.000000 apache-airflow-providers-asana-2.2.2rc1/apache_airflow_providers_asana.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:50.000000 apache-airflow-providers-asana-2.2.2rc1/apache_airflow_providers_asana.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-08-04 21:40:50.000000 apache-airflow-providers-asana-2.2.2rc1/apache_airflow_providers_asana.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:50.000000 apache-airflow-providers-asana-2.2.2rc1/apache_airflow_providers_asana.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-08-04 21:40:50.000000 apache-airflow-providers-asana-2.2.2rc1/apache_airflow_providers_asana.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:50.000000 apache-airflow-providers-asana-2.2.2rc1/apache_airflow_providers_asana.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-asana-2.2.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1938 2023-08-04 21:40:50.622283 apache-airflow-providers-asana-2.2.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1632 2023-08-04 21:40:49.000000 apache-airflow-providers-asana-2.2.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-asana-3.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1122 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-asana-3.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9024 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7480 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13369 2022-10-26 03:21:46.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/asana.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2022-09-14 19:22:24.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/asana_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9024 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      707 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       36 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-asana-3.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1832 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1460 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `apache-airflow-providers-asana-2.2.2rc1/LICENSE` & `apache-airflow-providers-asana-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.2rc1/MANIFEST.in` & `apache-airflow-providers-asana-3.0.0rc1/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 # `MANIFEST_TEMPLATE.py.jinja2` IN the `provider_packages` DIRECTORY
 
 
 
 
 include NOTICE
 include LICENSE
-include CHANGELOG.rst
+include CHANGELOG.txt
+include README.md
 global-exclude __pycache__  *.pyc
```

### Comparing `apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/get_provider_info.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/get_provider_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,29 +23,16 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-asana",
         "name": "Asana",
         "description": "`Asana <https://app.asana.com/>`__\n",
-        "suspended": False,
-        "versions": [
-            "2.2.2",
-            "2.2.1",
-            "2.2.0",
-            "2.1.0",
-            "2.0.1",
-            "2.0.0",
-            "1.1.3",
-            "1.1.2",
-            "1.1.1",
-            "1.1.0",
-            "1.0.0",
-        ],
-        "dependencies": ["apache-airflow>=2.4.0", "asana>=0.10,<4.0.0"],
+        "versions": ["3.0.0", "2.0.1", "2.0.0", "1.1.3", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
+        "dependencies": ["apache-airflow>=2.3.0", "asana>=0.10"],
         "integrations": [
             {
                 "integration-name": "Asana",
                 "external-doc-url": "https://developers.asana.com/docs",
                 "how-to-guide": ["/docs/apache-airflow-providers-asana/operators/asana.rst"],
                 "tags": ["software"],
             }
```

### Comparing `apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/hooks/__init__.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/hooks/asana.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/asana.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,29 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Connect to Asana."""
 from __future__ import annotations
 
-from functools import cached_property, wraps
+from functools import wraps
 from typing import Any
 
 from asana import Client  # type: ignore[attr-defined]
 from asana.error import NotFoundError  # type: ignore[attr-defined]
 
+from airflow.compat.functools import cached_property
 from airflow.hooks.base import BaseHook
 
 
 def _ensure_prefixes(conn_type):
-    """Remove when provider min airflow version >= 2.5.0 since this is now handled by provider manager."""
+    """
+    Remove when provider min airflow version >= 2.5.0 since this is handled by
+    provider manager from that version.
+    """
 
     def dec(func):
         @wraps(func)
         def inner():
             field_behaviors = func()
             conn_attrs = {"host", "schema", "login", "password", "port", "extra"}
 
@@ -81,41 +85,41 @@
         return extras.get(prefixed_name) or None
 
     def get_conn(self) -> Client:
         return self.client
 
     @staticmethod
     def get_connection_form_widgets() -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Returns connection widgets to add to connection form"""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import StringField
 
         return {
             "workspace": StringField(lazy_gettext("Workspace"), widget=BS3TextFieldWidget()),
             "project": StringField(lazy_gettext("Project"), widget=BS3TextFieldWidget()),
         }
 
     @staticmethod
     @_ensure_prefixes(conn_type="asana")
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Returns custom field behaviour"""
         return {
             "hidden_fields": ["port", "host", "login", "schema"],
             "relabeling": {},
             "placeholders": {
                 "password": "Asana personal access token",
                 "workspace": "Asana workspace gid",
                 "project": "Asana project gid",
             },
         }
 
     @cached_property
     def client(self) -> Client:
-        """Instantiates python-asana Client."""
+        """Instantiates python-asana Client"""
         if not self.connection.password:
             raise ValueError(
                 "Asana connection password must contain a personal access token: "
                 "https://developers.asana.com/docs/personal-access-token"
             )
 
         return Client.access_token(self.connection.password)
@@ -254,15 +258,15 @@
         self._validate_create_project_parameters(merged_params)
         response = self.client.projects.create(merged_params)
         return response
 
     @staticmethod
     def _validate_create_project_parameters(params: dict) -> None:
         """
-        Check that user provided the minimum required parameters for project creation.
+        Check that user provided the minimum required parameters for project creation
 
         :param params: Attributes that the new project should have
         :return: None; raises a ValueError if `params` does not contain the minimum required attributes.
         """
         required_parameters = {"workspace", "team"}
         if required_parameters.isdisjoint(params):
             raise ValueError(
```

### Comparing `apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/operators/__init__.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.2rc1/airflow/providers/asana/operators/asana_tasks.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/asana_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,19 +24,16 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class AsanaCreateTaskOperator(BaseOperator):
     """
-    This operator can be used to create Asana tasks.
-
-    .. seealso::
-        For more information on Asana optional task parameters:
-        https://developers.asana.com/docs/create-a-task
+    This operator can be used to create Asana tasks. For more information on
+    Asana optional task parameters, see https://developers.asana.com/docs/create-a-task
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:AsanaCreateTaskOperator`
 
     :param conn_id: The Asana connection to use.
     :param name: Name of the Asana task.
@@ -66,18 +63,16 @@
         self.log.info(response)
         return response["gid"]
 
 
 class AsanaUpdateTaskOperator(BaseOperator):
     """
     This operator can be used to update Asana tasks.
-
-    .. seealso::
-        For more information on Asana optional task parameters:
-        https://developers.asana.com/docs/update-a-task
+    For more information on Asana optional task parameters, see
+    https://developers.asana.com/docs/update-a-task
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:AsanaUpdateTaskOperator`
 
     :param conn_id: The Asana connection to use.
     :param asana_task_gid: Asana task ID to update
@@ -134,18 +129,15 @@
         response = hook.delete_task(self.asana_task_gid)
         self.log.info(response)
 
 
 class AsanaFindTaskOperator(BaseOperator):
     """
     This operator can be used to retrieve Asana tasks that match various filters.
-
-    .. seealso::
-        For a list of possible filters:
-        https://developers.asana.com/docs/update-a-task
+    See https://developers.asana.com/docs/update-a-task for a list of possible filters.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:AsanaFindTaskOperator`
 
     :param conn_id: The Asana connection to use.
     :param search_parameters: The parameters used to find relevant tasks. You must
```

### Comparing `apache-airflow-providers-asana-2.2.2rc1/apache_airflow_providers_asana.egg-info/SOURCES.txt` & `apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.2rc1/setup.cfg` & `apache-airflow-providers-asana-3.0.0rc1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -17,42 +17,41 @@
 	Environment :: Console
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	Framework :: Apache Airflow
 	Framework :: Apache Airflow :: Provider
 	License :: OSI Approved :: Apache Software License
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.2/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.2/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
 python_tag = py3
 
 [options]
 zip_safe = False
 include_package_data = True
-python_requires = ~=3.8
+python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0.dev0
-	asana>=0.10,<4.0.0
+	apache-airflow>=2.3.0.*
+	asana>=0.10
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.asana.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.asana
```

### Comparing `apache-airflow-providers-asana-2.2.2rc1/setup.py` & `apache-airflow-providers-asana-3.0.0rc1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,28 +22,21 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-asana package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "2.2.2"
+version = "3.0.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-asana setup."""
     setup(
         version=version,
         extras_require={},
-        packages=find_namespace_packages(
-            include=[
-                "airflow.providers.asana",
-                "airflow.providers.asana.*",
-                "airflow.providers.asana_vendor",
-                "airflow.providers.asana_vendor.*",
-            ],
-        ),
+        packages=find_namespace_packages(include=["airflow.providers.asana", "airflow.providers.asana.*"]),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

