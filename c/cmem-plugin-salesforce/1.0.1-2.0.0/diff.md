# Comparing `tmp/cmem_plugin_salesforce-1.0.1.tar.gz` & `tmp/cmem_plugin_salesforce-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_salesforce-1.0.1.tar", max compression
+gzip compressed data, was "cmem_plugin_salesforce-2.0.0.tar", max compression
```

## Comparing `cmem_plugin_salesforce-1.0.1.tar` & `cmem_plugin_salesforce-2.0.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    11334 2022-10-17 17:37:42.136711 cmem_plugin_salesforce-1.0.1/LICENSE
--rw-r--r--   0        0        0      370 2022-10-17 17:37:42.136711 cmem_plugin_salesforce-1.0.1/README-public.md
--rw-r--r--   0        0        0     1697 2022-10-17 17:37:42.136711 cmem_plugin_salesforce-1.0.1/cmem_plugin_salesforce/__init__.py
--rw-r--r--   0        0        0      302 2022-10-17 17:37:42.136711 cmem_plugin_salesforce-1.0.1/cmem_plugin_salesforce/helper/__init__.py
--rw-r--r--   0        0        0        0 2022-10-17 17:37:42.136711 cmem_plugin_salesforce-1.0.1/cmem_plugin_salesforce/workflow/__init__.py
--rw-r--r--   0        0        0     8311 2022-10-17 17:37:42.136711 cmem_plugin_salesforce-1.0.1/cmem_plugin_salesforce/workflow/operations.py
--rw-r--r--   0        0        0     7321 2022-10-17 17:37:42.136711 cmem_plugin_salesforce-1.0.1/cmem_plugin_salesforce/workflow/soql_query.py
--rw-r--r--   0        0        0     1670 2022-10-17 17:39:01.308321 cmem_plugin_salesforce-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 cmem_plugin_salesforce-1.0.1/setup.py
--rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 cmem_plugin_salesforce-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-08-08 07:51:54.458604 cmem_plugin_salesforce-2.0.0/LICENSE
+-rw-r--r--   0        0        0      370 2023-08-08 07:51:54.458604 cmem_plugin_salesforce-2.0.0/README-public.md
+-rw-r--r--   0        0        0     1697 2023-08-08 07:51:54.458604 cmem_plugin_salesforce-2.0.0/cmem_plugin_salesforce/__init__.py
+-rw-r--r--   0        0        0      302 2023-08-08 07:51:54.458604 cmem_plugin_salesforce-2.0.0/cmem_plugin_salesforce/helper/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:51:54.458604 cmem_plugin_salesforce-2.0.0/cmem_plugin_salesforce/workflow/__init__.py
+-rw-r--r--   0        0        0     8311 2023-08-08 07:51:54.458604 cmem_plugin_salesforce-2.0.0/cmem_plugin_salesforce/workflow/operations.py
+-rw-r--r--   0        0        0     6457 2023-08-08 07:51:54.458604 cmem_plugin_salesforce-2.0.0/cmem_plugin_salesforce/workflow/soql_query.py
+-rw-r--r--   0        0        0     1681 2023-08-08 07:52:29.266744 cmem_plugin_salesforce-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 cmem_plugin_salesforce-2.0.0/PKG-INFO
```

### Comparing `cmem_plugin_salesforce-1.0.1/LICENSE` & `cmem_plugin_salesforce-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_salesforce-1.0.1/cmem_plugin_salesforce/__init__.py` & `cmem_plugin_salesforce-2.0.0/cmem_plugin_salesforce/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_salesforce-1.0.1/cmem_plugin_salesforce/workflow/operations.py` & `cmem_plugin_salesforce-2.0.0/cmem_plugin_salesforce/workflow/operations.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_salesforce-1.0.1/cmem_plugin_salesforce/workflow/soql_query.py` & `cmem_plugin_salesforce-2.0.0/cmem_plugin_salesforce/workflow/soql_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,15 @@
     Entities,
 )
 from cmem_plugin_base.dataintegration.parameter.dataset import DatasetParameterType
 from cmem_plugin_base.dataintegration.parameter.multiline import (
     MultilineStringParameterType,
 )
 from cmem_plugin_base.dataintegration.plugins import WorkflowPlugin
-from cmem_plugin_base.dataintegration.types import BoolParameterType
 from cmem_plugin_base.dataintegration.utils import write_to_dataset
-from python_soql_parser import parse
 from simple_salesforce import Salesforce, SalesforceLogin
 
 from cmem_plugin_salesforce import (
     LINKS,
     USERNAME_DESCRIPTION,
     SECURITY_TOKEN_DESCRIPTION,
 )
@@ -59,15 +57,15 @@
 Retrieve first name and last name of all Contact resources. (with parser validation)
 ```
 {EXAMPLE_QUERY}
 ```
 
 Please refer to the {LINKS["OBJECT_REFERENCE"]} of the Salesforce Platform data
 model in order to get an overview of the available objects and fields.
-"""
+"""  # nosec
 
 PARSE_SOQL_DESCRIPTION = f"""
 Parse query text for validation.
 
 To avoid mistakes, the plugin tries to validate the given query text before sending it
 to Salesforce. Turn off this feature, in case you are encountering false validation
 errors. You can always validate your query in the {LINKS["DEV_CONSOLE"]}.
@@ -78,26 +76,14 @@
 
 SOQL uses the SELECT statement combined with filtering statements to return sets
 of data, which can optionally be ordered. For a complete description of the syntax,
 see {LINKS["SOQL_SYNTAX"]}.
 """
 
 
-def validate_soql(soql_query: str):
-    """Validate SOQL"""
-    try:
-        parse(soql_query=soql_query)
-    except Exception as error:
-        raise ValueError(
-            "We failed to validate the syntax of your SOQL query. "
-            "Please fix your SOQL query or disable the validation in case you know "
-            "what you do (see advanced options in the task configuration)."
-        ) from error
-
-
 def validate_credentials(username: str, password: str, security_token: str):
     """Validate Salesforce login credentials"""
     SalesforceLogin(username=username, password=password, security_token=security_token)
 
 
 def get_projections(record: OrderedDict) -> list[str]:
     """get keys from dict"""
@@ -140,46 +126,34 @@
             description="In addition to have direct output of the fetched entities of"
             " your SOQL query, you can directly write the response to a"
             " JSON dataset (mostly for debugging purpose).",
             param_type=DatasetParameterType(dataset_type="json"),
             advanced=True,
             default_value="",
         ),
-        PluginParameter(
-            name="parse_soql",
-            label="Parse SOQL Query",
-            description=PARSE_SOQL_DESCRIPTION,
-            param_type=BoolParameterType(),
-            advanced=True,
-            default_value=True,
-        ),
     ],
 )
 class SoqlQuery(WorkflowPlugin):
     """Salesforce Integration Plugin"""
 
     # pylint: disable-msg=too-many-arguments
     def __init__(
         self,
         username: str,
         password: str,
         security_token: str,
         soql_query: str,
         dataset: str = "",
-        parse_soql: bool = False,
     ) -> None:
         validate_credentials(username, password, security_token)
 
         self.dataset = dataset
         self.username = username
         self.password = password
         self.security_token = security_token
-        if parse_soql:
-            validate_soql(soql_query)
-
         self.soql_query = soql_query
 
     def execute(
         self, inputs: Sequence[Entities], context: ExecutionContext
     ) -> Entities:
         self.log.info("Start Salesforce Plugin")
         salesforce = Salesforce(
```

### Comparing `cmem_plugin_salesforce-1.0.1/pyproject.toml` & `cmem_plugin_salesforce-2.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 [tool.poetry]
 name = "cmem-plugin-salesforce"
-version = "1.0.1"
+version = "2.0.0"
 license = "Apache-2.0"
 description = "Send or receive data from your organization´s Salesforce account."
 authors = ["Sai Ranga Reddy Nukala <rangareddy.nukala@eccenca.com>"]
 homepage = "https://github.com/eccenca/cmem-plugin-salesforce"
 classifiers = [
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 readme = "README-public.md"
 keywords = [
     "eccenca Corporate Memory", "plugin", "Salesforce"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-cmem-plugin-base = "^2.1.0"
+python = "^3.11"
+cmem-plugin-base = "^4.0.0"
 simple-salesforce = "^1.11.6"
-python-soql-parser = "^0.1.11"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.0"
-pytest-dependency = "^0.5.1"
-pytest-cov = "^3.0.0"
-black = "^22.1.0"
-bandit = "^1.7.2"
+bandit = "^1.7.5"
+black = "^23.3.0"
+coverage = "^7.2.3"
+defusedxml = "^0.7.1"
+flake8-formatter-junit-xml = "^0.0.6"
+genbadge = "^1.1.0"
+mypy = "^1.2.0"
+pillow = "^9.5.0"
 pylint-junit = "^0.3.2"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+pytest-memray = "^1.4.0"
 safety = "^1.10.3"
-genbadge = "^1.0.6"
-flake8-formatter-junit-xml = "^0.0.6"
-typed-ast = "^1.5.2"
-mypy = "^0.931"
-coverage = "^6.3.2"
-defusedxml = "^0.7.1"
-requests = "^2.28.1"
+typed-ast = "^1.5.4"
+wheel = "^0.38.4"
+types-requests = "^2.31.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
@@ -64,8 +65,7 @@
 
 [tool.mypy]
 warn_return_any = true
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 addopts = ""
-
```

### Comparing `cmem_plugin_salesforce-1.0.1/PKG-INFO` & `cmem_plugin_salesforce-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-salesforce
-Version: 1.0.1
+Version: 2.0.0
 Summary: Send or receive data from your organization´s Salesforce account.
 Home-page: https://github.com/eccenca/cmem-plugin-salesforce
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,Salesforce
 Author: Sai Ranga Reddy Nukala
 Author-email: rangareddy.nukala@eccenca.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cmem-plugin-base (>=2.1.0,<3.0.0)
-Requires-Dist: python-soql-parser (>=0.1.11,<0.2.0)
+Requires-Dist: cmem-plugin-base (>=4.0.0,<5.0.0)
 Requires-Dist: simple-salesforce (>=1.11.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-salesforce
 
 Send or receive data from your organization´s Salesforce account.
```

