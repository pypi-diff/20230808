# Comparing `tmp/forestadmin_agent_toolkit-1.0.0b5.tar.gz` & `tmp/forestadmin_agent_toolkit-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_toolkit-1.0.0b5.tar", max compression
+gzip compressed data, was "forestadmin_agent_toolkit-1.0.0b6.tar", max compression
```

## Comparing `forestadmin_agent_toolkit-1.0.0b5.tar` & `forestadmin_agent_toolkit-1.0.0b6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/README.md
--rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/__init__.py
--rw-r--r--   0        0        0     5682 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/agent.py
--rw-r--r--   0        0        0      135 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/exceptions.py
--rw-r--r--   0        0        0     1276 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/forest_logger.py
--rw-r--r--   0        0        0      909 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/options.py
--rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/actions/__init__.py
--rw-r--r--   0        0        0     2292 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/actions/requests.py
--rw-r--r--   0        0        0     6431 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/actions/resources.py
--rw-r--r--   0        0        0      464 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/base.py
--rw-r--r--   0        0        0      913 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/__init__.py
--rw-r--r--   0        0        0     2816 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/charts_collection.py
--rw-r--r--   0        0        0     1966 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
--rw-r--r--   0        0        0    17087 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/crud.py
--rw-r--r--   0        0        0    21321 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/crud_related.py
--rw-r--r--   0        0        0     2972 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/decorators.py
--rw-r--r--   0        0        0      148 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/exceptions.py
--rw-r--r--   0        0        0    11045 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/filter.py
--rw-r--r--   0        0        0     5624 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/requests.py
--rw-r--r--   0        0        0     9929 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/stats.py
--rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/security/__init__.py
--rw-r--r--   0        0        0      144 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/security/exceptions.py
--rw-r--r--   0        0        0     3763 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/security/resources.py
--rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/__init__.py
--rw-r--r--   0        0        0     8403 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/permissions/__init__.py
--rw-r--r--   0        0        0      264 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/permissions/options.py
--rw-r--r--   0        0        0     1660 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/serializers/__init__.py
--rw-r--r--   0        0        0     9523 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/serializers/json_api.py
--rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     3227 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/authentication.py
--rw-r--r--   0        0        0     4044 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/context.py
--rw-r--r--   0        0        0     1392 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/csv.py
--rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
--rw-r--r--   0        0        0     3039 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
--rw-r--r--   0        0        0     4367 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
--rw-r--r--   0        0        0     2236 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
--rw-r--r--   0        0        0     4508 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
--rw-r--r--   0        0        0     2288 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
--rw-r--r--   0        0        0     7847 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
--rw-r--r--   0        0        0      506 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
--rw-r--r--   0        0        0     3057 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/type.py
--rw-r--r--   0        0        0     1281 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/validation.py
--rw-r--r--   0        0        0     4265 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/http.py
--rw-r--r--   0        0        0     1683 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/id.py
--rw-r--r--   0        0        0      541 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/token.py
--rw-r--r--   0        0        0     1771 2023-08-01 13:28:40.426165 forestadmin_agent_toolkit-1.0.0b5/pyproject.toml
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-08 13:37:34.069918 forestadmin_agent_toolkit-1.0.0b6/README.md
+-rw-r--r--   0        0        0        0 2023-08-08 13:37:34.069918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/__init__.py
+-rw-r--r--   0        0        0     5682 2023-08-08 13:37:34.069918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/agent.py
+-rw-r--r--   0        0        0      135 2023-08-08 13:37:34.069918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/exceptions.py
+-rw-r--r--   0        0        0     1276 2023-08-08 13:37:34.069918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/forest_logger.py
+-rw-r--r--   0        0        0      909 2023-08-08 13:37:34.069918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/options.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/actions/__init__.py
+-rw-r--r--   0        0        0     2292 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/actions/requests.py
+-rw-r--r--   0        0        0     6431 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/actions/resources.py
+-rw-r--r--   0        0        0      464 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/base.py
+-rw-r--r--   0        0        0      913 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/__init__.py
+-rw-r--r--   0        0        0     2816 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/charts_collection.py
+-rw-r--r--   0        0        0     1966 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
+-rw-r--r--   0        0        0    17087 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/crud.py
+-rw-r--r--   0        0        0    21321 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/crud_related.py
+-rw-r--r--   0        0        0     2972 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/decorators.py
+-rw-r--r--   0        0        0      148 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/exceptions.py
+-rw-r--r--   0        0        0    11217 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/filter.py
+-rw-r--r--   0        0        0     5624 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/requests.py
+-rw-r--r--   0        0        0     9929 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/stats.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/security/__init__.py
+-rw-r--r--   0        0        0      144 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/security/exceptions.py
+-rw-r--r--   0        0        0     3763 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/security/resources.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/services/__init__.py
+-rw-r--r--   0        0        0     8403 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/services/permissions/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/services/permissions/options.py
+-rw-r--r--   0        0        0     1660 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/services/serializers/__init__.py
+-rw-r--r--   0        0        0     9523 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/services/serializers/json_api.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     3227 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/authentication.py
+-rw-r--r--   0        0        0     4044 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/context.py
+-rw-r--r--   0        0        0     1392 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/csv.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
+-rw-r--r--   0        0        0     3039 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
+-rw-r--r--   0        0        0     4367 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
+-rw-r--r--   0        0        0     2236 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
+-rw-r--r--   0        0        0     4508 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
+-rw-r--r--   0        0        0     2288 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
+-rw-r--r--   0        0        0     7847 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
+-rw-r--r--   0        0        0      506 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
+-rw-r--r--   0        0        0     3057 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/type.py
+-rw-r--r--   0        0        0     1281 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/validation.py
+-rw-r--r--   0        0        0     4265 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/http.py
+-rw-r--r--   0        0        0     1683 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/id.py
+-rw-r--r--   0        0        0      541 2023-08-08 13:37:34.073918 forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/token.py
+-rw-r--r--   0        0        0     1771 2023-08-08 13:37:59.301727 forestadmin_agent_toolkit-1.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.0.0b6/PKG-INFO
```

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/agent.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/agent.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/forest_logger.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/forest_logger.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/options.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/options.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/actions/requests.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/actions/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/actions/resources.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/actions/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/__init__.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/charts_collection.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/charts_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/charts_datasource.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/charts_datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/crud.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/crud.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/crud_related.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/crud_related.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/decorators.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/decorators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/filter.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,18 @@
     if not filters and request.body and "filters" in request.body:
         filters = request.body["filters"]
     if not filters:
         return None
 
     jsoned_filters = json.loads(filters)
     try:
-        jsoned_filters["value"] = _parse_value(jsoned_filters, request.collection)
+        if isinstance(request, RequestRelationCollection):
+            jsoned_filters["value"] = _parse_value(jsoned_filters, request.foreign_collection)
+        else:
+            jsoned_filters["value"] = _parse_value(jsoned_filters, request.collection)
         condition_tree = ConditionTreeFactory.from_plain_object(jsoned_filters)
     except ConditionTreeFactoryException as e:
         raise FilterException(str(e))
 
     try:
         ConditionTreeValidator.validate(condition_tree, _get_collection(request))
     except ConditionTreeValidatorException as e:
```

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/requests.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/stats.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/collections/stats.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/security/resources.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/resources/security/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/permissions/__init__.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/services/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/serializers/__init__.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/services/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/serializers/json_api.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/services/serializers/json_api.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/authentication.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/context.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/csv.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/csv.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/action_values.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/action_values.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/emitter.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/emitter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/filterable.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/filterable.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/type.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/type.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/validation.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/forest_schema/validation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/http.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/http.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/id.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/id.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/token.py` & `forestadmin_agent_toolkit-1.0.0b6/forestadmin/agent_toolkit/utils/token.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b5/pyproject.toml` & `forestadmin_agent_toolkit-1.0.0b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-toolkit"
-version = "1.0.0-beta.5"
+version = "1.0.0-beta.6"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 typing-extensions = ">=4.2.0, <5.0"
 tzdata = "~2022.6"
 aiohttp = "~=3.8"
 oic = "~=1.4"
 python-jose = ">=3.3, <4.0"
 cachetools = "~=5.2"
 marshmallow-jsonapi = ">=0.24.0, <1.0"
-forestadmin-datasource-toolkit = "^1.0.0-beta.5"
+forestadmin-datasource-toolkit = "^1.0.0-beta.6"
 [[tool.poetry.dependencies.pandas]]
 version = "<=1.1.5"
 python = "<3.7.1"
 
 [[tool.poetry.dependencies.pandas]]
 version = ">=1.3.4,<=1.3.5"
 python = ">=3.7.1,<3.8"
```

### Comparing `forestadmin_agent_toolkit-1.0.0b5/PKG-INFO` & `forestadmin_agent_toolkit-1.0.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-toolkit
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: cachetools (>=5.2,<6.0)
-Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.5,<2.0.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.6,<2.0.0)
 Requires-Dist: marshmallow-jsonapi (>=0.24.0,<1.0)
 Requires-Dist: oic (>=1.4,<2.0)
 Requires-Dist: pandas (<=1.1.5) ; python_full_version < "3.7.1"
 Requires-Dist: pandas (>=1.3.4,<=1.3.5) ; python_full_version >= "3.7.1" and python_version < "3.8"
 Requires-Dist: pandas (>=1.4.0) ; python_version >= "3.8"
 Requires-Dist: python-jose (>=3.3,<4.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0)
```

