# Comparing `tmp/promql_http_api-0.2.2.tar.gz` & `tmp/promql_http_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promql_http_api-0.2.2.tar", max compression
+gzip compressed data, was "promql_http_api-0.3.0.tar", max compression
```

## Comparing `promql_http_api-0.2.2.tar` & `promql_http_api-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    10764 2023-01-27 09:07:19.549411 promql_http_api-0.2.2/LICENSE.md
--rw-r--r--   0        0        0     5829 2023-07-08 05:56:13.452605 promql_http_api-0.2.2/README.md
--rw-r--r--   0        0        0      746 2023-01-27 09:07:19.565408 promql_http_api-0.2.2/promql_http_api/__init__.py
--rw-r--r--   0        0        0     1049 2023-01-27 09:07:19.816418 promql_http_api-0.2.2/promql_http_api/alerts.py
--rw-r--r--   0        0        0     1070 2023-01-27 09:07:19.833422 promql_http_api-0.2.2/promql_http_api/alertsmanagers.py
--rw-r--r--   0        0        0     3388 2023-07-06 19:53:17.638030 promql_http_api-0.2.2/promql_http_api/api.py
--rw-r--r--   0        0        0     1724 2023-01-27 09:07:19.827419 promql_http_api-0.2.2/promql_http_api/api_endpoint.py
--rw-r--r--   0        0        0     4527 2023-03-31 07:15:17.659745 promql_http_api-0.2.2/promql_http_api/api_response.py
--rw-r--r--   0        0        0     1065 2023-01-27 09:07:19.831419 promql_http_api-0.2.2/promql_http_api/buildinfo.py
--rw-r--r--   0        0        0     1056 2023-01-27 09:07:19.829418 promql_http_api-0.2.2/promql_http_api/config.py
--rw-r--r--   0        0        0     1053 2023-01-27 09:07:19.850430 promql_http_api-0.2.2/promql_http_api/flags.py
--rw-r--r--   0        0        0     1190 2023-01-27 09:07:19.812420 promql_http_api-0.2.2/promql_http_api/format_query.py
--rw-r--r--   0        0        0       44 2023-07-08 03:05:34.339332 promql_http_api-0.2.2/promql_http_api/http_config.py
--rw-r--r--   0        0        0     1344 2023-01-27 09:37:30.210288 promql_http_api-0.2.2/promql_http_api/label_values.py
--rw-r--r--   0        0        0     1068 2023-01-27 09:37:38.611318 promql_http_api-0.2.2/promql_http_api/labels.py
--rw-r--r--   0        0        0     6844 2023-07-08 05:37:13.396655 promql_http_api-0.2.2/promql_http_api/query.py
--rw-r--r--   0        0        0     1246 2023-01-27 09:07:19.818421 promql_http_api-0.2.2/promql_http_api/rules.py
--rw-r--r--   0        0        0     1071 2023-01-27 09:07:19.840413 promql_http_api-0.2.2/promql_http_api/runtimeinfo.py
--rw-r--r--   0        0        0     1497 2023-01-27 09:33:47.634307 promql_http_api-0.2.2/promql_http_api/series.py
--rw-r--r--   0        0        0     1257 2023-01-27 09:07:19.825417 promql_http_api-0.2.2/promql_http_api/targets.py
--rw-r--r--   0        0        0     1209 2023-07-08 05:56:43.764691 promql_http_api-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6975 1970-01-01 00:00:00.000000 promql_http_api-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    10764 2023-01-27 09:07:19.549411 promql_http_api-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     7248 2023-08-08 03:23:49.919661 promql_http_api-0.3.0/README.md
+-rw-r--r--   0        0        0      746 2023-01-27 09:07:19.565408 promql_http_api-0.3.0/promql_http_api/__init__.py
+-rw-r--r--   0        0        0     1049 2023-01-27 09:07:19.816418 promql_http_api-0.3.0/promql_http_api/alerts.py
+-rw-r--r--   0        0        0     1070 2023-01-27 09:07:19.833422 promql_http_api-0.3.0/promql_http_api/alertsmanagers.py
+-rw-r--r--   0        0        0     3555 2023-07-11 00:34:11.623046 promql_http_api-0.3.0/promql_http_api/api.py
+-rw-r--r--   0        0        0     1724 2023-01-27 09:07:19.827419 promql_http_api-0.3.0/promql_http_api/api_endpoint.py
+-rw-r--r--   0        0        0     4527 2023-03-31 07:15:17.659745 promql_http_api-0.3.0/promql_http_api/api_response.py
+-rw-r--r--   0        0        0     1065 2023-01-27 09:07:19.831419 promql_http_api-0.3.0/promql_http_api/buildinfo.py
+-rw-r--r--   0        0        0     1056 2023-01-27 09:07:19.829418 promql_http_api-0.3.0/promql_http_api/config.py
+-rw-r--r--   0        0        0     1053 2023-01-27 09:07:19.850430 promql_http_api-0.3.0/promql_http_api/flags.py
+-rw-r--r--   0        0        0     1190 2023-01-27 09:07:19.812420 promql_http_api-0.3.0/promql_http_api/format_query.py
+-rw-r--r--   0        0        0       44 2023-07-08 03:05:34.339332 promql_http_api-0.3.0/promql_http_api/http_config.py
+-rw-r--r--   0        0        0     1344 2023-01-27 09:37:30.210288 promql_http_api-0.3.0/promql_http_api/label_values.py
+-rw-r--r--   0        0        0     1068 2023-01-27 09:37:38.611318 promql_http_api-0.3.0/promql_http_api/labels.py
+-rw-r--r--   0        0        0     7417 2023-08-07 20:29:26.630663 promql_http_api-0.3.0/promql_http_api/query.py
+-rw-r--r--   0        0        0     1246 2023-01-27 09:07:19.818421 promql_http_api-0.3.0/promql_http_api/rules.py
+-rw-r--r--   0        0        0     1071 2023-01-27 09:07:19.840413 promql_http_api-0.3.0/promql_http_api/runtimeinfo.py
+-rw-r--r--   0        0        0     1497 2023-01-27 09:33:47.634307 promql_http_api-0.3.0/promql_http_api/series.py
+-rw-r--r--   0        0        0     1257 2023-01-27 09:07:19.825417 promql_http_api-0.3.0/promql_http_api/targets.py
+-rw-r--r--   0        0        0     1209 2023-08-08 03:25:26.738878 promql_http_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8394 1970-01-01 00:00:00.000000 promql_http_api-0.3.0/PKG-INFO
```

### Comparing `promql_http_api-0.2.2/LICENSE.md` & `promql_http_api-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/README.md` & `promql_http_api-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -75,14 +75,36 @@
 # with 5 retries and retry intervals of 5, 10, 20, and 40 seconds
 promql_response_data = q(retries=5, timeout=5, backoff=2)
 
 # Convert the cached result to a DataFrame
 df = q.to_dataframe()
 ```
 
+### Working with schemas
+
+The `to_dataframe()` method takes an optional `schema` parameter. The schema is a dictionary that controls several elements of the query. A schema may include the following element keys: `columns`, `dtype`, and `timezone`.
+
+The `columns` element controls the PromQL response elements to be included as columns in the returned DataFrame. The returned DataFrame will always include a timestamp column (in seconds since the epoch), and a `value` column. If `columns` is not provided, all the fields returned in a PromQL response will be included in the returned DataFrame. If `columns` is provided, only the fields listed in `columns` will be included in the returned DataFrame.
+
+The `dtype` element controls the data type of the `value` column in the returned DataFrame. The default is `str`. The `dtype` element may be set to any valid Pandas data type.
+
+The `timezone` element allows the user to request an additional `datetime` column which is formatted in the specified timezone. The `timezone` element must be a timezone object from the [pytz](https://pypi.org/project/pytz/) library. If the `timezone` element is not provided, the returned DataFrame will not include a `datetime` column.
+
+Here is an example of how to use a schema:
+```python
+schema = {
+    'columns': ['node', 'sensor'],
+    'dtype': float,
+    'timezone': pytz.timezone('US/Eastern')
+}
+
+df = q.to_dataframe(schema)
+```
+
+
 ## Debugging
 
 If something goes wrong, you can look at the HTTP response and the PromQL response information. Here are some examples:
 ```python
 from promql_http_api import PromqlHttpApi
 api = PromqlHttpApi('http://localhost:9090')
 tz = pytz.timezone('UTC')
```

### Comparing `promql_http_api-0.2.2/promql_http_api/__init__.py` & `promql_http_api-0.3.0/promql_http_api/__init__.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/alerts.py` & `promql_http_api-0.3.0/promql_http_api/alerts.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/alertsmanagers.py` & `promql_http_api-0.3.0/promql_http_api/alertsmanagers.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/api.py` & `promql_http_api-0.3.0/promql_http_api/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,90 +35,90 @@
     Provides a convenient function interface to instanciate
     API endpoint classes
     '''
 
     def __init__(self, url: str):
         self.url = url
 
-    def query(self, *args, **kwargs):
+    def query(self, *args, **kwargs) -> Query:
         '''
         Get a Query object
         '''
         return Query(self.url, *args, **kwargs)
 
-    def query_range(self, *args, **kwargs):
+    def query_range(self, *args, **kwargs) -> QueryRange:
         '''
         Get a QueryRange object
         '''
         return QueryRange(self.url, *args, **kwargs)
 
-    def format_query(self, *args, **kwargs):
+    def format_query(self, *args, **kwargs) -> FormatQuery:
         '''
         Get a FormatQuery object
         '''
         return FormatQuery(self.url, *args, **kwargs)
 
-    def series(self, *args, **kwargs):
+    def series(self, *args, **kwargs) -> Series:
         '''
         Get a Series object
         '''
         return Series(self.url, *args, **kwargs)
 
-    def labels(self, *args, **kwargs):
+    def labels(self, *args, **kwargs) -> Labels:
         '''
         Get a Labels object
         '''
         return Labels(self.url, *args, **kwargs)
 
-    def label_values(self, *args, **kwargs):
+    def label_values(self, *args, **kwargs) -> LabelValues:
         '''
         Get a LabelValues object
         '''
         return LabelValues(self.url, *args, **kwargs)
 
-    def targets(self, *args, **kwargs):
+    def targets(self, *args, **kwargs) -> Targets:
         '''
         Get a Targets object
         '''
         return Targets(self.url, *args, **kwargs)
 
-    def rules(self, *args, **kwargs):
+    def rules(self, *args, **kwargs) -> Rules:
         '''
         Get a Rules object
         '''
         return Rules(self.url, *args, **kwargs)
 
-    def alerts(self, *args, **kwargs):
+    def alerts(self, *args, **kwargs) -> Alerts:
         '''
         Get an Alerts object
         '''
         return Alerts(self.url, *args, **kwargs)
 
-    def alertmanagers(self, *args, **kwargs):
+    def alertmanagers(self, *args, **kwargs) -> AlertManagers:
         '''
         Get an AlertManagers object
         '''
         return AlertManagers(self.url, *args, **kwargs)
 
-    def config(self, *args, **kwargs):
+    def config(self, *args, **kwargs) -> Config:
         '''
         Get a Config object
         '''
         return Config(self.url, *args, **kwargs)
 
-    def flags(self, *args, **kwargs):
+    def flags(self, *args, **kwargs) -> Flags:
         '''
         Get a Flags object
         '''
         return Flags(self.url, *args, **kwargs)
 
-    def runtimeinfo(self, *args, **kwargs):
+    def runtimeinfo(self, *args, **kwargs) -> RuntimeInfo:
         '''
         Get a RuntimeInfo object
         '''
         return RuntimeInfo(self.url, *args, **kwargs)
 
-    def buildinfo(self, *args, **kwargs):
+    def buildinfo(self, *args, **kwargs) -> BuildInfo:
         '''
         Get a BuildInfo object
         '''
         return BuildInfo(self.url, *args, **kwargs)
```

### Comparing `promql_http_api-0.2.2/promql_http_api/api_endpoint.py` & `promql_http_api-0.3.0/promql_http_api/api_endpoint.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/api_response.py` & `promql_http_api-0.3.0/promql_http_api/api_response.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/buildinfo.py` & `promql_http_api-0.3.0/promql_http_api/buildinfo.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/config.py` & `promql_http_api-0.3.0/promql_http_api/config.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/flags.py` & `promql_http_api-0.3.0/promql_http_api/flags.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/format_query.py` & `promql_http_api-0.3.0/promql_http_api/format_query.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/label_values.py` & `promql_http_api-0.3.0/promql_http_api/label_values.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/labels.py` & `promql_http_api-0.3.0/promql_http_api/labels.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/query.py` & `promql_http_api-0.3.0/promql_http_api/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 class Base(ApiEndpoint):
     '''
     Base class for Query and QueryRange endpoints
     '''
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.logger = logging.getLogger(f"{__name__}::{self.__class__.__name__}")
+        self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
         self.timezone = timezone.utc
         self.time_format = "%Y-%m-%dT%H:%M:%S"
         self.schema = None
         self.prom_results = {}
 
     def to_dataframe(self) -> DataFrame:
         '''
@@ -62,51 +62,63 @@
             return self._vector_to_dataframe()
         elif prom_result_type == 'matrix':
             return self._matrix_to_dataframe()
         else:
             raise ValueError(f"Unexpected PromQL result type: {prom_result_type}")
 
     def _vector_to_dataframe(self) -> DataFrame:
-        '''
-        Helper function to convert a vector result to a Pandas DataFrame
-        '''
         records = []
         columns = self.get_schema_columns()
+        df_has_datetime = (self.schema and 'timezone' in self.schema.keys())
         for result in self.prom_results:
             prom_metric = result['metric']
             columns = columns if columns else list(prom_metric.keys())
             record = [prom_metric[column] for column in columns]
             value = result['value']
-            pd_timestamp = Timestamp(value[0], unit='s', tz=self.timezone)
-            result = self.cast(value[1])
-            full_record = [pd_timestamp] + record + [result]
-            self.logger.debug(f'record = {full_record}')
+            full_record = self._make_full_record(value, record, df_has_datetime)
             records.append(full_record)
-        columns = ['timestamp'] + columns + ['value']
+        if df_has_datetime:
+            columns = ['timestamp'] + columns + ['value']
+        else:
+            columns = ['timestamp', 'datetime'] + columns + ['value']
         df = DataFrame(records, columns=columns)
         return df
 
     def _matrix_to_dataframe(self):
         records = []
         columns = self.get_schema_columns()
+        df_has_datetime = (self.schema and 'timezone' in self.schema.keys())
         for result in self.prom_results:
             prom_metric = result['metric']
-            values = result['values']
             columns = columns if columns else list(prom_metric.keys())
             record = [prom_metric[column] for column in columns]
+            values = result['values']
             for value in values:
-                pd_timestamp = Timestamp(value[0], unit='s', tz=self.timezone)
-                result = self.cast(value[1])
-                full_record = [pd_timestamp] + record + [result]
-                self.logger.debug(f'record = {full_record}')
+                full_record = self._make_full_record(value, record, df_has_datetime)
                 records.append(full_record)
-        columns = ['timestamp'] + columns + ['value']
+        if df_has_datetime:
+            columns = ['timestamp', 'datetime'] + columns + ['value']
+        else:
+            columns = ['timestamp'] + columns + ['value']
         df = DataFrame(records, columns=columns)
         return df
 
+    def _make_full_record(self, value, partial_record, df_has_datetime):
+        full_record = []
+        timestamp = value[0]
+        result = self.cast(value[1])
+        if df_has_datetime:
+            pd_timestamp = Timestamp(timestamp, unit='s', tz=self.timezone)
+            full_record = [timestamp, pd_timestamp] + partial_record + [result]
+        else:
+            full_record = [timestamp] + partial_record + [result]
+
+        self.logger.debug(f'record = {full_record}')
+        return full_record
+
     def get_schema_columns(self) -> list[str]:
         if self.schema:
             return self.schema.get('columns', [])
         else:
             return []
 
     def cast(self, result):
@@ -122,15 +134,15 @@
     '''
 
     def __init__(self,
                  url: str = "",
                  query: str = "",
                  time: datetime = datetime.now()):
         super().__init__(url)
-        self.logger = logging.getLogger(f"{__name__}::{self.__class__.__name__}")
+        self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
         self.logger.debug(f"url = {url}; query = {query}; time = {time}")
         self.query = query
         self.time = time
 
     def __str__(self):
         return self.query
 
@@ -168,15 +180,15 @@
     def __init__(self,
                  url: str,
                  query: str,
                  start: datetime,
                  end: datetime,
                  step: str):
         super().__init__(url)
-        self.logger = logging.getLogger(f"{__name__}::{self.__class__.__name__}")
+        self.logger = logging.getLogger(f"{__name__}.{self.__class__.__name__}")
         self.logger.debug(f'query = {query}; start = {start}; end = {end}; step = {step}')
         self.query = query
         self.start = start
         self.end = end
         self.step = step
 
     def __str__(self):
@@ -199,13 +211,13 @@
         url = '/api/v1/query_range?query=' + self.query
         url += '&start=' + start
         url += '&end=' + end
         url += '&step=' + self.step
         self.logger.debug(f'returned url = {url}')
         return url
 
-    def to_dataframe(self, schema: dict = {}):
+    def to_dataframe(self, schema: dict = {}) -> DataFrame:
         if self.query is None:
-            return None
+            raise ValueError("Please set the QueryRange::query element to issue a PromQL HTTP API query")
         self.schema = schema
         self.__call__()
         return super().to_dataframe()
```

### Comparing `promql_http_api-0.2.2/promql_http_api/rules.py` & `promql_http_api-0.3.0/promql_http_api/rules.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/runtimeinfo.py` & `promql_http_api-0.3.0/promql_http_api/runtimeinfo.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/series.py` & `promql_http_api-0.3.0/promql_http_api/series.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/promql_http_api/targets.py` & `promql_http_api-0.3.0/promql_http_api/targets.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.2.2/pyproject.toml` & `promql_http_api-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promql-http-api"
-version = "0.2.2"
+version = "0.3.0"
 description = "Query a Prometheus server and get a Pandas DataFrame"
 homepage = "https://github.com/nir-arad/promql-http-api"
 repository = "https://github.com/nir-arad/promql-http-api"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["prometheus", "promql", "pandas", "dataframe"]
 authors = ["Nir Arad"]
```

### Comparing `promql_http_api-0.2.2/PKG-INFO` & `promql_http_api-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promql-http-api
-Version: 0.2.2
+Version: 0.3.0
 Summary: Query a Prometheus server and get a Pandas DataFrame
 Home-page: https://github.com/nir-arad/promql-http-api
 License: Apache-2.0
 Keywords: prometheus,promql,pandas,dataframe
 Author: Nir Arad
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -102,14 +102,36 @@
 # with 5 retries and retry intervals of 5, 10, 20, and 40 seconds
 promql_response_data = q(retries=5, timeout=5, backoff=2)
 
 # Convert the cached result to a DataFrame
 df = q.to_dataframe()
 ```
 
+### Working with schemas
+
+The `to_dataframe()` method takes an optional `schema` parameter. The schema is a dictionary that controls several elements of the query. A schema may include the following element keys: `columns`, `dtype`, and `timezone`.
+
+The `columns` element controls the PromQL response elements to be included as columns in the returned DataFrame. The returned DataFrame will always include a timestamp column (in seconds since the epoch), and a `value` column. If `columns` is not provided, all the fields returned in a PromQL response will be included in the returned DataFrame. If `columns` is provided, only the fields listed in `columns` will be included in the returned DataFrame.
+
+The `dtype` element controls the data type of the `value` column in the returned DataFrame. The default is `str`. The `dtype` element may be set to any valid Pandas data type.
+
+The `timezone` element allows the user to request an additional `datetime` column which is formatted in the specified timezone. The `timezone` element must be a timezone object from the [pytz](https://pypi.org/project/pytz/) library. If the `timezone` element is not provided, the returned DataFrame will not include a `datetime` column.
+
+Here is an example of how to use a schema:
+```python
+schema = {
+    'columns': ['node', 'sensor'],
+    'dtype': float,
+    'timezone': pytz.timezone('US/Eastern')
+}
+
+df = q.to_dataframe(schema)
+```
+
+
 ## Debugging
 
 If something goes wrong, you can look at the HTTP response and the PromQL response information. Here are some examples:
 ```python
 from promql_http_api import PromqlHttpApi
 api = PromqlHttpApi('http://localhost:9090')
 tz = pytz.timezone('UTC')
```

