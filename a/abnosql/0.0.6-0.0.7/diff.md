# Comparing `tmp/abnosql-0.0.6.tar.gz` & `tmp/abnosql-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abnosql-0.0.6.tar", last modified: Mon Jul 31 17:37:48 2023, max compression
+gzip compressed data, was "abnosql-0.0.7.tar", last modified: Tue Aug  8 20:09:40 2023, max compression
```

## Comparing `abnosql-0.0.6.tar` & `abnosql-0.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.860376 abnosql-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 17:37:28.000000 abnosql-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-07-31 17:37:48.860376 abnosql-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-07-31 17:37:28.000000 abnosql-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.856377 abnosql-0.0.6/abnosql/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4128 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/kms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.856377 abnosql-0.0.6/abnosql/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/mocks/mock_azure_kms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/mocks/mock_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/mocks/mock_dynamodbx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.856377 abnosql-0.0.6/abnosql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.860376 abnosql-0.0.6/abnosql/plugins/kms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/kms/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/kms/azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.860376 abnosql-0.0.6/abnosql/plugins/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/table/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/table/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/table/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/table.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.856377 abnosql-0.0.6/abnosql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 17:37:48.860376 abnosql-0.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2818 2023-07-31 17:37:28.000000 abnosql-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:09:40.968374 abnosql-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-08 20:09:25.000000 abnosql-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-08-08 20:09:40.968374 abnosql-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-08-08 20:09:25.000000 abnosql-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:09:40.964374 abnosql-0.0.7/abnosql/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4128 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/kms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:09:40.968374 abnosql-0.0.7/abnosql/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/mocks/mock_azure_kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/mocks/mock_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/mocks/mock_dynamodbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:09:40.968374 abnosql-0.0.7/abnosql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:09:40.968374 abnosql-0.0.7/abnosql/plugins/kms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/plugins/kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/plugins/kms/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/plugins/kms/azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:09:40.968374 abnosql-0.0.7/abnosql/plugins/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/plugins/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/plugins/table/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/plugins/table/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/plugins/table/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 20:09:25.000000 abnosql-0.0.7/abnosql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:09:40.968374 abnosql-0.0.7/abnosql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-08-08 20:09:40.000000 abnosql-0.0.7/abnosql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-08 20:09:40.000000 abnosql-0.0.7/abnosql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:09:40.000000 abnosql-0.0.7/abnosql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 20:09:40.000000 abnosql-0.0.7/abnosql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-08 20:09:40.000000 abnosql-0.0.7/abnosql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 20:09:40.000000 abnosql-0.0.7/abnosql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 20:09:40.968374 abnosql-0.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2818 2023-08-08 20:09:25.000000 abnosql-0.0.7/setup.py
```

### Comparing `abnosql-0.0.6/LICENSE` & `abnosql-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.6/PKG-INFO` & `abnosql-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abnosql
-Version: 0.0.6
+Version: 0.0.7
 Summary: NoSQL Abstraction Library
 Home-page: https://github.com/rog555/abnosql
 Download-URL: http://pypi.python.org/pypi/abnosql
 Author: Roger Foskett
 Author-email: r_foskett@hotmail.com
 Maintainer: Roger Foskett
 Maintainer-email: r_foskett@hotmail.com
```

### Comparing `abnosql-0.0.6/README.md` & `abnosql-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.6/abnosql/cli.py` & `abnosql-0.0.7/abnosql/cli.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.6/abnosql/kms.py` & `abnosql-0.0.7/abnosql/kms.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,8 +115,12 @@
     """
     if provider is None:
         provider = os.environ.get('ABNOSQL_KMS')
     pm = plugin.get_pm('kms')
     module = pm.get_plugin(provider)
     if module is None:
         raise ex.PluginException(f'kms.{provider} plugin not found')
+    if hasattr(module, 'MISSING_DEPS'):
+        raise ex.PluginException(
+            f'kms.{provider} plugin missing dependencies'
+        )
     return module.Kms(pm, config)
```

### Comparing `abnosql-0.0.6/abnosql/mocks/mock_azure_kms.py` & `abnosql-0.0.7/abnosql/mocks/mock_azure_kms.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.6/abnosql/mocks/mock_cosmos.py` & `abnosql-0.0.7/abnosql/mocks/mock_cosmos.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
 
     def _callback(request):
         path = urlparse.urlsplit(request.url).path
         headers = dict(request.headers)
 
         def _response(code=404, body=None, _headers=None):
             return (
-                code, _headers or {}, json.dumps({
+                code, _headers or {
+                    'Content-Type': 'application/json'
+                }, json.dumps({
                     "Errors": [
                         "Resource Not Found. "
                         "Learn more: https://aka.ms/cosmosdb-tsg-not-found"
                     ]
                 }) if code == 404
                 else json.dumps(body) if body is not None
                 else body
```

### Comparing `abnosql-0.0.6/abnosql/mocks/mock_dynamodbx.py` & `abnosql-0.0.7/abnosql/mocks/mock_dynamodbx.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.6/abnosql/plugin.py` & `abnosql-0.0.7/abnosql/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from importlib import import_module
 import os
 from pkgutil import iter_modules
 import typing as t
 
 import pluggy  # type: ignore
 
-from abnosql.exceptions import PluginException
-
 
 PKG_ROOT = os.path.dirname(os.path.abspath(__file__))
 PKG_NAME = os.path.basename(PKG_ROOT)
 _PMS = {}  # type: ignore
 
 
 class PluginSpec:
@@ -90,18 +88,14 @@
     spec_module = getattr(entity_module, f'{prefix}Specs', None)
     if spec_module and issubclass(spec_module, PluginSpec):  # type: ignore
         pm.add_hookspecs(spec_module)
 
     for info in iter_modules([os.path.join(PKG_ROOT, 'plugins', entity)]):
         path = f'{PKG_NAME}.plugins.{entity}.{info.name}'
         module = import_module(path)
-        if hasattr(module, 'MISSING_DEPS'):
-            raise PluginException(
-                f'plugin {path} missing required dependencies'
-            )
         pm.register(plugin=module, name=info.name)
 
     pm.load_setuptools_entrypoints(f'{PKG_NAME}.{entity}')
     pm.check_pending()
 
     if not nocache:
         _PMS[entity] = pm  # type: ignore
```

### Comparing `abnosql-0.0.6/abnosql/plugins/kms/aws.py` & `abnosql-0.0.7/abnosql/plugins/kms/aws.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.6/abnosql/plugins/kms/azure.py` & `abnosql-0.0.7/abnosql/plugins/kms/azure.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.6/abnosql/plugins/table/cosmos.py` & `abnosql-0.0.7/abnosql/plugins/table/cosmos.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,16 @@
 
     @cosmos_ex_handler()
     def query(
         self,
         key: t.Optional[t.Dict[str, t.Any]] = None,
         filters: t.Optional[t.Dict[str, t.Any]] = None,
         limit: t.Optional[int] = None,
-        next: t.Optional[str] = None
+        next: t.Optional[str] = None,
+        index: t.Optional[str] = None
     ) -> t.Dict[str, t.Any]:
         filters = filters or {}
         key = key or {}
         validate_query_attrs(key, filters)
         parameters = {
             f'@{k}': v
             for k, v in filters.items()
```

### Comparing `abnosql-0.0.6/abnosql/plugins/table/dynamodb.py` & `abnosql-0.0.7/abnosql/plugins/table/dynamodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,16 @@
     )
     return {_type: str(val)}
 
 
 def get_dynamodb_kwargs(
     name: str,
     key: t.Optional[t.Dict[str, t.Any]] = None,
-    filters: t.Optional[t.Dict[str, t.Any]] = None
+    filters: t.Optional[t.Dict[str, t.Any]] = None,
+    index: t.Optional[str] = None
 ) -> t.Dict:
     key = key or {}
     if len(key) > 2:
         raise ValueError('key length must be 1 or 2')
     filters = filters or {}
     validate_query_attrs(key, filters)
 
@@ -121,14 +122,16 @@
         _names[f'#{k}'] = k
         _values[f':{k}'] = v
 
     kwargs: t.Dict[str, t.Any] = {
         'TableName': name,
         'Select': 'ALL_ATTRIBUTES'
     }
+    if index is not None:
+        kwargs['IndexName'] = index
     if len(key):
         kwargs['KeyConditionExpression'] = ' AND '.join([
             f'{k} = :{k}' for k in key.keys()
         ])
     if len(_values):
         kwargs['ExpressionAttributeValues'] = _values
     if len(_names):
@@ -241,18 +244,19 @@
 
     @dynamodb_ex_handler()
     def query(
         self,
         key: t.Optional[t.Dict[str, t.Any]] = None,
         filters: t.Optional[t.Dict[str, t.Any]] = None,
         limit: t.Optional[int] = None,
-        next: t.Optional[str] = None
+        next: t.Optional[str] = None,
+        index: t.Optional[str] = None
     ) -> t.Dict[str, t.Any]:
         kwargs = get_dynamodb_kwargs(
-            self.name, key, filters
+            self.name, key, filters=filters, index=index
         )
         if next is not None:
             kwargs['ExclusiveStartKey'] = json.loads(b64decode(next).decode())
         if limit is not None:
             kwargs['Limit'] = limit
         response = None
         if key is not None:
```

### Comparing `abnosql-0.0.6/abnosql/plugins/table/memory.py` & `abnosql-0.0.7/abnosql/plugins/table/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,16 @@
 
     @memory_ex_handler()
     def query(
         self,
         key: t.Dict[str, t.Any],
         filters: t.Optional[t.Dict[str, t.Any]] = None,
         limit: t.Optional[int] = None,
-        next: t.Optional[str] = None
+        next: t.Optional[str] = None,
+        index: t.Optional[str] = None
     ) -> t.Dict[str, t.Any]:
         filters = filters or {}
         validate_query_attrs(key, filters)
         parameters = {
             f'@{k}': v
             for k, v in filters.items()
         }
```

### Comparing `abnosql-0.0.6/abnosql/table.py` & `abnosql-0.0.7/abnosql/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,24 +182,26 @@
 
     @abstractmethod
     def query(
         self,
         key: t.Optional[t.Dict[str, t.Any]] = None,
         filters: t.Optional[t.Dict[str, t.Any]] = None,
         limit: t.Optional[int] = None,
-        next: t.Optional[str] = None
+        next: t.Optional[str] = None,
+        index: t.Optional[str] = None
     ) -> t.Dict[str, t.Any]:
         """Perform key based query with optional exact match filters
 
         Args:
 
             key: dictionary containing partition key and range/sort key
             filters: optional dictionary of key=value to query and filter on
             limit: query limit
             next: pagination token
+            index: name of index to use (dynamodb only)
 
         Returns:
             dictionary containing 'items' and 'next' pagination token
 
         """
         pass
 
@@ -546,14 +548,18 @@
                 database = _database
                 break
 
     pm = plugin.get_pm('table')
     module = pm.get_plugin(database)
     if module is None:
         raise ex.PluginException(f'table.{database} plugin not found')
+    if hasattr(module, 'MISSING_DEPS'):
+        raise ex.PluginException(
+            f'table.{database} plugin missing dependencies'
+        )
     if not isinstance(config, dict):
         config = {}
     _module = module.Table(pm, name, config)
 
     # load crypto module
     kcfg = config.get('kms')
     if isinstance(kcfg, dict):
@@ -573,15 +579,15 @@
         if 'session' in config and 'session' not in kcfg:
             # aws_encryption_sdk uses botocore session
             config['kms']['session'] = config['session']._session
 
         # check required attrs
         missing = [
             _ for _ in ['attrs', 'key_attrs']
-            if not isinstance(kcfg[_], list) or len(kcfg[_]) == 0
+            if not isinstance(kcfg.get(_), list) or len(kcfg[_]) == 0
         ]
         if len(missing):
             raise ex.ConfigException(
                 'kms config missing %s' % ', '.join(missing)
             )
 
     return _module
```

### Comparing `abnosql-0.0.6/abnosql.egg-info/PKG-INFO` & `abnosql-0.0.7/abnosql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abnosql
-Version: 0.0.6
+Version: 0.0.7
 Summary: NoSQL Abstraction Library
 Home-page: https://github.com/rog555/abnosql
 Download-URL: http://pypi.python.org/pypi/abnosql
 Author: Roger Foskett
 Author-email: r_foskett@hotmail.com
 Maintainer: Roger Foskett
 Maintainer-email: r_foskett@hotmail.com
```

### Comparing `abnosql-0.0.6/abnosql.egg-info/SOURCES.txt` & `abnosql-0.0.7/abnosql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.6/abnosql.egg-info/requires.txt` & `abnosql-0.0.7/abnosql.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.6/setup.py` & `abnosql-0.0.7/setup.py`

 * *Files identical despite different names*

