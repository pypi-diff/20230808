# Comparing `tmp/macrometa-source-collection-0.0.56.tar.gz` & `tmp/macrometa-source-collection-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.56.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.57.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.56.tar` & `macrometa-source-collection-0.0.57.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    11137 2023-07-14 08:38:33.443026 macrometa-source-collection-0.0.56/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0    10411 2023-07-14 08:38:33.443026 macrometa-source-collection-0.0.56/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-07-14 08:38:33.711036 macrometa-source-collection-0.0.56/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.56/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.56/PKG-INFO
+-rw-r--r--   0        0        0    11140 2023-08-08 03:18:14.647447 macrometa-source-collection-0.0.57/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0    11991 2023-08-08 03:18:14.647447 macrometa-source-collection-0.0.57/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     4101 2023-08-08 03:18:14.647447 macrometa-source-collection-0.0.57/macrometa_source_collection/util.py
+-rw-r--r--   0        0        0     1625 2023-08-08 03:18:14.891464 macrometa-source-collection-0.0.57/pyproject.toml
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.57/setup.py
+-rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.57/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.56/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.57/macrometa_source_collection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """GDN data connector source for GDN Collections."""
+import time
 from collections import defaultdict
 from urllib.parse import urlparse
 
 import pkg_resources
 import singer
-import time
 from c8 import C8Client
 from c8connector import C8Connector, Sample, ConfigProperty, ConfigAttributeType, Schema, SchemaAttributeType, \
     SchemaAttribute, ValidationException
 from singer import utils
 from singer.catalog import Catalog, CatalogEntry
 from singer.schema import Schema as SingerSchema
 
@@ -51,15 +51,15 @@
         """Returns the logo image for the connector."""
         return ""
 
     def validate(self, integration: dict) -> None:
         """Validate given configurations against the connector.
         If invalid, throw an exception with the cause.
         """
-        try: 
+        try:
             config = self.get_config(integration)
             cursor_batch_size = int(config["cursor_batch_size"])
             if not 0 < cursor_batch_size <= 1024:
                 raise ValidationException(f"Invalid `cursor_batch_size` value `{cursor_batch_size}` provided.")
             cursor_ttl = int(config["cursor_ttl"])
             if not 30 <= cursor_ttl <= 120:
                 raise ValidationException(f"Invalid `cursor_ttl` value `{cursor_ttl}` provided.")
@@ -224,15 +224,16 @@
         host=config["gdn_host"],
         port=443,
         geofabric=config["fabric"],
         apikey=config["api_key"]
     ), collection_name, 50, workflow_run)
     schema_properties = {
         k: SingerSchema(
-            type=['null', 'string', 'integer', 'number', 'boolean', 'array', 'object'] if v == 'null' else (v if k == '_key' else ['null', v]),
+            type=['null', 'string', 'integer', 'number', 'boolean', 'array', 'object'] if v == 'null' else (
+                v if k == '_key' else ['null', v]),
             format=None
         )
         for k, v in schema.items()
     }
     # inject `_sdc_deleted_at` prop to the schema.
     schema_properties['_sdc_deleted_at'] = SingerSchema(type=['null', 'string'], format='date-time')
     singer_schema = SingerSchema(type='object', properties=schema_properties)
@@ -247,17 +248,17 @@
     return catalog
 
 
 def dump_catalog(catalog: Catalog):
     catalog.dump()
 
 
-def do_sync(conn_config, catalog, default_replication_method):
-    client = GDNCollectionClient(conn_config)
-    client.sync(catalog.streams[0])
+def do_sync(conn_config, catalog, state):
+    gdn_client = GDNCollectionClient(conn_config)
+    gdn_client.sync(catalog.streams[0], state)
 
 
 def extract_gdn_host(url):
     parsed_url = urlparse(url)
     if parsed_url.scheme:
         resource_name = parsed_url.netloc.strip()
     else:
@@ -273,15 +274,16 @@
                    'gdn_host': extract_gdn_host(args.config['gdn_host']),
                    'fabric': args.config['fabric'],
                    'source_collection': args.config['source_collection']}
 
     if args.discover:
         do_discovery(conn_config, workflow_run=True)
     elif args.catalog:
-        do_sync(conn_config, args.catalog, args.config.get('default_replication_method'))
+        state = args.state or {}
+        do_sync(conn_config, args.catalog, state)
     else:
         LOGGER.info("No properties were selected")
     return
 
 
 def main():
     try:
```

### Comparing `macrometa-source-collection-0.0.56/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.57/macrometa_source_collection/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Manage GDN collection streams"""
-
 import json
 import logging
 import os
 import time
 import uuid
 
 import pulsar
 import singer
 from c8 import C8Client
 from prometheus_client import start_http_server, Counter
 from singer import utils
 from singer.catalog import CatalogEntry
 
+from macrometa_source_collection.util import start_acknowledgment_task, MSG_ACK_BATCH_SIZE, write_to_state, \
+    KEY_LAST_MSG_ID, KEY_FULL_TABLE_COMPLETED
+
 LOGGER = singer.get_logger('macrometa_source_collection')
 
 region_label = os.getenv("GDN_FEDERATION", "NA")
 tenant_label = os.getenv("GDN_TENANT", "NA")
 fabric_label = os.getenv("GDN_FABRIC", "NA")
 workflow_label = os.getenv("WORKFLOW_UUID", "NA")
 metric_service_url = os.getenv("METRIC_SERVICE_API")
 is_metrics_enabled = os.getenv("MACROMETA_SOURCE_COLLECTION_IS_METRICS_ENABLED", 'False')
 
+
 class GDNCollectionClient:
     """Client for handling GDN collection streams."""
 
     def __init__(self, config) -> None:
         """Init new GDN Collection Client."""
         self._host = config.get("gdn_host")
         self._fabric = config.get("fabric")
@@ -47,126 +50,156 @@
 
         try:
             # try to enable collection stream on the source collection.
             self._c8_client.update_collection_properties(self._collection, has_stream=True)
         except:
             pass
 
-        self.exported_bytes = Counter("exported_bytes", "Total number of bytes exported from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
-        self.exported_documents = Counter("exported_documents", "Total number of documents exported from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
-        self.export_errors = Counter("export_errors", "Total count of errors while exporting data from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
+        self.exported_bytes = Counter("exported_bytes", "Total number of bytes exported from GDN collections",
+                                      ['region', 'tenant', 'fabric', 'workflow'])
+        self.exported_documents = Counter("exported_documents",
+                                          "Total number of documents exported from GDN collections",
+                                          ['region', 'tenant', 'fabric', 'workflow'])
+        self.export_errors = Counter("export_errors", "Total count of errors while exporting data from GDN collections",
+                                     ['region', 'tenant', 'fabric', 'workflow'])
         if is_metrics_enabled.lower() == 'false':
             self.ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion',
-                        ['region', 'tenant', 'fabric', 'workflow'])
+                                         ['region', 'tenant', 'fabric', 'workflow'])
         # Start the Prometheus HTTP server for exposing metrics
         LOGGER.info("Macrometa collection source is starting the metrics server.")
         start_http_server(8000)
 
-    def sync(self, stream):
+    def sync(self, stream, state):
         """Return documents in target GDN collection as records."""
         if self._c8_client.has_collection(self._collection):
             self.send_schema_message(stream)
             columns = list(stream.schema.properties.keys())
             columns.remove("_sdc_deleted_at")
             schema_properties = stream.schema.properties
-            # pulsar client throws some messages into stdout when subscribed to a topic. Meltano tap/target doesn't like
-            # this and tries to process the pulsar log messages in stdout as input singer records. Therefore we are trying
-            #  to turn off pulsar logging here. This is the best way I found with the current pulsar client API.
+            # When subscribed to a topic, the Pulsar client may output some log messages to stdout.
+            # However, Meltano tap/target processes these log messages as input singer records,
+            # which can lead to unexpected behavior.
+            # To prevent this issue, we disable Pulsar logging here to ensure a clean data flow.
             _pulsar_logger = logging.getLogger("pulsar-logger")
             _pulsar_logger.setLevel(logging.CRITICAL)
             _pulsar_logger.addHandler(logging.NullHandler())
 
-            # Create a consumer before hand so as to capture changes done while loading existing data
+            # Create a consumer beforehand to capture changes done while loading existing data
             _pulsar_client = pulsar.Client(
                 f"pulsar+ssl://{self._host}:6651/",
                 authentication=self._auth,
                 tls_allow_insecure_connection=False,
                 logger=_pulsar_logger,
             )
             _sub_name = self._wf_uuid if self._wf_uuid else f"cs_{uuid.uuid1()}"
             _topic = f"persistent://{self._tenant}/c8local.{self._fabric}/{self._collection}"
-            _consumer: pulsar.Consumer = _pulsar_client.subscribe(_topic, _sub_name, initial_position=pulsar.InitialPosition.Earliest)
-
-            # Load existing data
-            self.load_existing_data(stream, columns, schema_properties)
-            LOGGER.info("Full table sync completed.")
+            _consumer: pulsar.Consumer = _pulsar_client.subscribe(
+                _topic, _sub_name, initial_position=pulsar.InitialPosition.Earliest)
 
-            # Change data capture
+            # Initiate full table sync
+            full_table_completed = singer.get_bookmark(state, self._collection, KEY_FULL_TABLE_COMPLETED)
+            if full_table_completed:
+                LOGGER.info("Full table sync already completed.")
+            else:
+                LOGGER.info("Full table sync started.")
+                self.load_existing_data(stream, columns, schema_properties)
+                full_table_completed = True
+                state = write_to_state(state, self._collection, KEY_FULL_TABLE_COMPLETED, full_table_completed)
+                LOGGER.info("Full table sync completed.")
+
+            # Initiate CDC sync
+            LOGGER.info("CDC sync started.")
+            start_acknowledgment_task(self._collection, _consumer)
+            _consumer.redeliver_unacknowledged_messages()
+            un_ack_msgs = 0
             while True:
-                try: 
+                try:
                     msg = _consumer.receive()
                     time_extracted = utils.now()
                     data = msg.data()
-                    if data == None or not data:
+                    if data is None or not data:
                         continue
                     props = msg.properties()
                     j = json.loads(data.decode("utf8"))
                     j.pop('_id', None)
                     j.pop('_rev', None)
-                    record_sent =  False
+                    record_sent = False
                     if props["op"] == "INSERT" or props["op"] == "UPDATE":
                         # skip inserts not having valid schema
                         if len(j.keys() ^ columns) == 0 and all(
-                            j[key] is None or (isinstance(schema_properties[key].type, list) and get_singer_data_type(j[key]) in schema_properties[key].type)
-                                                 or (isinstance(schema_properties[key].type, str) and get_singer_data_type(j[key]) == schema_properties[key].type)
-                            for key in j.keys()
+                                j[key] is None or (
+                                        isinstance(schema_properties[key].type, list) and get_singer_data_type(
+                                    j[key]) in schema_properties[key].type)
+                                or (isinstance(schema_properties[key].type, str) and get_singer_data_type(j[key]) ==
+                                    schema_properties[key].type)
+                                for key in j.keys()
                         ):
                             j['_sdc_deleted_at'] = None
                             singer_record = self.msg_to_singer_message(stream, j, None, time_extracted)
                             singer.write_message(singer_record)
                             record_sent = True
                         else:
                             LOGGER.warn("The record: %s, does not match the most common schema. Skipping it..", j)
                     elif props["op"] == "DELETE":
                         # Currently, we don't have a way to validate schema here
                         j.pop('_delete', None)
                         j['_sdc_deleted_at'] = singer.utils.strftime(utils.now())
                         singer_record = self.msg_to_singer_message(stream, j, None, time_extracted)
                         singer.write_message(singer_record)
                         record_sent = True
-                    _consumer.acknowledge(msg.message_id())
-                    if is_metrics_enabled.lower() == 'true' and record_sent:
-                        self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(j)))
-                        self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+
+                    if record_sent:
+                        un_ack_msgs += 1
+                        if un_ack_msgs == MSG_ACK_BATCH_SIZE:
+                            state = write_to_state(state, self._collection, KEY_LAST_MSG_ID,
+                                                   msg.message_id().serialize())
+                            un_ack_msgs = 0
+                        if is_metrics_enabled.lower() == 'true':
+                            self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(
+                                len(json.dumps(j)))
+                            self.exported_documents.labels(region_label, tenant_label, fabric_label,
+                                                           workflow_label).inc()
                 except Exception as e:
                     LOGGER.warn(f"Exception received: {e}")
                     if is_metrics_enabled.lower() == 'false':
                         self.ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                     else:
                         self.export_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                     raise e
-        
         else:
             raise FileNotFoundError("Collection {} not found".format(self._collection))
 
-
     def load_existing_data(self, stream, columns, schema_properties):
         cursor = self._c8_client._fabric.c8ql.execute(f"FOR d IN @@collection RETURN d",
                                                       bind_vars={"@collection": self._collection}, stream=True,
                                                       batch_size=self._cursor_batch_size, ttl=self._cursor_ttl)
         try:
             while (not cursor.empty()) or cursor.has_more():
                 rec = cursor.next()
                 time_extracted = utils.now()
                 rec.pop('_id', None)
                 rec.pop('_rev', None)
                 # skip existing data not having valid schema
                 if len(rec.keys() ^ columns) == 0 and all(
-                    rec[key] is None or (isinstance(schema_properties[key].type, list) and get_singer_data_type(rec[key]) in schema_properties[key].type)
-                                         or (isinstance(schema_properties[key].type, str) and get_singer_data_type(rec[key]) == schema_properties[key].type)
-                    for key in rec.keys()
+                        rec[key] is None or (
+                                isinstance(schema_properties[key].type, list) and get_singer_data_type(rec[key]) in
+                                schema_properties[key].type)
+                        or (isinstance(schema_properties[key].type, str) and get_singer_data_type(rec[key]) ==
+                            schema_properties[key].type)
+                        for key in rec.keys()
                 ):
                     singer_record = self.msg_to_singer_message(stream, rec, None, time_extracted)
                     start_time = time.time()
                     singer.write_message(singer_record)
                     end_time = time.time()
                     if end_time - start_time > 10:
                         LOGGER.warn(f"Took {end_time - start_time}seconds to write record:{singer_record}")
                     if is_metrics_enabled.lower() == 'true':
-                        self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(rec)))
+                        self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(
+                            len(json.dumps(rec)))
                         self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 else:
                     LOGGER.warn("The record: %s, does not match the most common schema. Skipping it..", rec)
         except Exception as e:
             time.sleep(100)
             raise e
```

### Comparing `macrometa-source-collection-0.0.56/pyproject.toml` & `macrometa-source-collection-0.0.57/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.56'
+version='0.0.57'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -30,15 +30,15 @@
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
 c8connector = ">=0.0.24"
 chardet = "4.0.0"
 idna = "2.10"
 numpy = "1.21.6"
 pandas = "1.3.5"
-pyC8 = "0.17.3"
+pyC8 = "1.0.1"
 requests = "2.25.1"
 websocket-client = "0.57.0"
 pulsar-client = "2.10.1"
 prometheus-client = "0.16.0"
 
 [tool.poetry.scripts]
 # CLI declaration
```

### Comparing `macrometa-source-collection-0.0.56/setup.py` & `macrometa-source-collection-0.0.57/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
  'chardet==4.0.0',
  'idna==2.10',
  'numpy==1.21.6',
  'pandas==1.3.5',
  'pipelinewise-singer-python==1.2.0',
  'prometheus-client==0.16.0',
  'pulsar-client==2.10.1',
- 'pyC8==0.17.3',
+ 'pyC8==1.0.1',
  'requests==2.25.1',
  'websocket-client==0.57.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.56',
+    'version': '0.0.57',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.56/PKG-INFO` & `macrometa-source-collection-0.0.57/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.56
+Version: 0.0.57
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,11 +18,11 @@
 Requires-Dist: chardet (==4.0.0)
 Requires-Dist: idna (==2.10)
 Requires-Dist: numpy (==1.21.6)
 Requires-Dist: pandas (==1.3.5)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
 Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: pulsar-client (==2.10.1)
-Requires-Dist: pyC8 (==0.17.3)
+Requires-Dist: pyC8 (==1.0.1)
 Requires-Dist: requests (==2.25.1)
 Requires-Dist: websocket-client (==0.57.0)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-collection/issues
```

