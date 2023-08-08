# Comparing `tmp/cloudquery-plugin-pb-0.0.14.tar.gz` & `tmp/cloudquery-plugin-pb-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudquery-plugin-pb-0.0.14.tar", last modified: Fri Jul 28 08:22:47 2023, max compression
+gzip compressed data, was "cloudquery-plugin-pb-0.0.15.tar", last modified: Tue Aug  8 14:00:22 2023, max compression
```

## Comparing `cloudquery-plugin-pb-0.0.14.tar` & `cloudquery-plugin-pb-0.0.15.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:47.495581 cloudquery-plugin-pb-0.0.14/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-28 08:22:47.495581 cloudquery-plugin-pb-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:47.487582 cloudquery-plugin-pb-0.0.14/cloudquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:47.491582 cloudquery-plugin-pb-0.0.14/cloudquery/discovery_v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/cloudquery/discovery_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/cloudquery/discovery_v1/discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/cloudquery/discovery_v1/discovery_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/cloudquery/discovery_v1/discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/cloudquery/discovery_v1/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:47.491582 cloudquery-plugin-pb-0.0.14/cloudquery/plugin_v3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/cloudquery/plugin_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/cloudquery/plugin_v3/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/cloudquery/plugin_v3/plugin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/cloudquery/plugin_v3/plugin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/cloudquery/plugin_v3/plugin_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/cloudquery/plugin_v3/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:47.495581 cloudquery-plugin-pb-0.0.14/cloudquery_plugin_pb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-28 08:22:47.000000 cloudquery-plugin-pb-0.0.14/cloudquery_plugin_pb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-28 08:22:47.000000 cloudquery-plugin-pb-0.0.14/cloudquery_plugin_pb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:22:47.000000 cloudquery-plugin-pb-0.0.14/cloudquery_plugin_pb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 08:22:47.000000 cloudquery-plugin-pb-0.0.14/cloudquery_plugin_pb.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:22:47.000000 cloudquery-plugin-pb-0.0.14/cloudquery_plugin_pb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 08:22:47.000000 cloudquery-plugin-pb-0.0.14/cloudquery_plugin_pb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 08:22:47.000000 cloudquery-plugin-pb-0.0.14/cloudquery_plugin_pb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 08:22:47.495581 cloudquery-plugin-pb-0.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-28 08:22:31.000000 cloudquery-plugin-pb-0.0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:00:22.927448 cloudquery-plugin-pb-0.0.15/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-08 14:00:22.927448 cloudquery-plugin-pb-0.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:00:22.923448 cloudquery-plugin-pb-0.0.15/cloudquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:00:22.923448 cloudquery-plugin-pb-0.0.15/cloudquery/discovery_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/cloudquery/discovery_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/cloudquery/discovery_v1/discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/cloudquery/discovery_v1/discovery_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/cloudquery/discovery_v1/discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/cloudquery/discovery_v1/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:00:22.927448 cloudquery-plugin-pb-0.0.15/cloudquery/plugin_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/cloudquery/plugin_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/cloudquery/plugin_v3/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/cloudquery/plugin_v3/plugin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/cloudquery/plugin_v3/plugin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/cloudquery/plugin_v3/plugin_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/cloudquery/plugin_v3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:00:22.927448 cloudquery-plugin-pb-0.0.15/cloudquery_plugin_pb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-08 14:00:22.000000 cloudquery-plugin-pb-0.0.15/cloudquery_plugin_pb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-08 14:00:22.000000 cloudquery-plugin-pb-0.0.15/cloudquery_plugin_pb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:00:22.000000 cloudquery-plugin-pb-0.0.15/cloudquery_plugin_pb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 14:00:22.000000 cloudquery-plugin-pb-0.0.15/cloudquery_plugin_pb.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:00:22.000000 cloudquery-plugin-pb-0.0.15/cloudquery_plugin_pb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 14:00:22.000000 cloudquery-plugin-pb-0.0.15/cloudquery_plugin_pb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 14:00:22.000000 cloudquery-plugin-pb-0.0.15/cloudquery_plugin_pb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 14:00:22.927448 cloudquery-plugin-pb-0.0.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-08 14:00:03.000000 cloudquery-plugin-pb-0.0.15/setup.py
```

### Comparing `cloudquery-plugin-pb-0.0.14/LICENSE` & `cloudquery-plugin-pb-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.14/PKG-INFO` & `cloudquery-plugin-pb-0.0.15/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-pb
-Version: 0.0.14
+Version: 0.0.15
 Summary: CloudQuery Plugin client and server library
 Home-page: https://github.com/cloudquery/plugin-pb-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-pb-0.0.14/README.md` & `cloudquery-plugin-pb-0.0.15/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # plugin-pb-python
 
-This is a low-level auto-generate gRPC client and server for CloudQuery plugin from [plugin-pb protos](https://github.com/cloudquery/plugin-pb).
+This is a low-level auto-generated gRPC client and server for CloudQuery plugin from [plugin-pb protos](https://github.com/cloudquery/plugin-pb).
 
 ## Development
 
 ### Prerequisites
 
 - [Python 3.7+](https://www.python.org/downloads/)
```

### Comparing `cloudquery-plugin-pb-0.0.14/cloudquery/discovery_v1/discovery_pb2.py` & `cloudquery-plugin-pb-0.0.15/cloudquery/discovery_v1/discovery_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'cloudquery/discovery_v1/discovery.proto\x12\x17\x63loudquery.discovery.v1\"6\n\x0bGetVersions\x1a\t\n\x07Request\x1a\x1c\n\x08Response\x12\x10\n\x08versions\x18\x01 \x03(\x05\x32w\n\tDiscovery\x12j\n\x0bGetVersions\x12,.cloudquery.discovery.v1.GetVersions.Request\x1a-.cloudquery.discovery.v1.GetVersions.ResponseB>Z<github.com/cloudquery/plugin-pb-go/pb/discovery/v1;discoveryb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'cloudquery/discovery_v1/discovery.proto\x12\x17\x63loudquery.discovery.v1\"6\n\x0bGetVersions\x1a\t\n\x07Request\x1a\x1c\n\x08Response\x12\x10\n\x08versions\x18\x01 \x03(\x05\x32w\n\tDiscovery\x12j\n\x0bGetVersions\x12,.cloudquery.discovery.v1.GetVersions.Request\x1a-.cloudquery.discovery.v1.GetVersions.ResponseB\\\n\x1aio.cloudquery.discovery.v1P\x01Z<github.com/cloudquery/plugin-pb-go/pb/discovery/v1;discoveryb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'cloudquery.discovery_v1.discovery_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z<github.com/cloudquery/plugin-pb-go/pb/discovery/v1;discovery'
+  DESCRIPTOR._serialized_options = b'\n\032io.cloudquery.discovery.v1P\001Z<github.com/cloudquery/plugin-pb-go/pb/discovery/v1;discovery'
   _globals['_GETVERSIONS']._serialized_start=68
   _globals['_GETVERSIONS']._serialized_end=122
   _globals['_GETVERSIONS_REQUEST']._serialized_start=83
   _globals['_GETVERSIONS_REQUEST']._serialized_end=92
   _globals['_GETVERSIONS_RESPONSE']._serialized_start=94
   _globals['_GETVERSIONS_RESPONSE']._serialized_end=122
   _globals['_DISCOVERY']._serialized_start=124
```

### Comparing `cloudquery-plugin-pb-0.0.14/cloudquery/discovery_v1/discovery_pb2.pyi` & `cloudquery-plugin-pb-0.0.15/cloudquery/discovery_v1/discovery_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.14/cloudquery/discovery_v1/discovery_pb2_grpc.py` & `cloudquery-plugin-pb-0.0.15/cloudquery/discovery_v1/discovery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.14/cloudquery/plugin_v3/arrow.py` & `cloudquery-plugin-pb-0.0.15/cloudquery/plugin_v3/arrow.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.14/cloudquery/plugin_v3/plugin_pb2.py` & `cloudquery-plugin-pb-0.0.15/cloudquery/plugin_v3/plugin_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!cloudquery/plugin_v3/plugin.proto\x12\x14\x63loudquery.plugin.v3\x1a\x1fgoogle/protobuf/timestamp.proto\".\n\x07GetName\x1a\t\n\x07Request\x1a\x18\n\x08Response\x12\x0c\n\x04name\x18\x01 \x01(\t\"4\n\nGetVersion\x1a\t\n\x07Request\x1a\x1b\n\x08Response\x12\x0f\n\x07version\x18\x01 \x01(\t\"B\n\x04Init\x1a.\n\x07Request\x12\x0c\n\x04spec\x18\x01 \x01(\x0c\x12\x15\n\rno_connection\x18\x02 \x01(\x08\x1a\n\n\x08Response\"W\n\tGetTables\x1a.\n\x07Request\x12\x0e\n\x06tables\x18\x01 \x03(\t\x12\x13\n\x0bskip_tables\x18\x02 \x03(\t\x1a\x1a\n\x08Response\x12\x0e\n\x06tables\x18\x01 \x03(\x0c\"\xcd\x03\n\x04Sync\x1a\x1f\n\rMessageInsert\x12\x0e\n\x06record\x18\x01 \x01(\x0c\x1a$\n\x13MessageMigrateTable\x12\r\n\x05table\x18\x01 \x01(\x0c\x1a\x38\n\x0e\x42\x61\x63kendOptions\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x12\n\nconnection\x18\x02 \x01(\t\x1a\xa6\x01\n\x07Request\x12\x0e\n\x06tables\x18\x01 \x03(\t\x12\x13\n\x0bskip_tables\x18\x02 \x03(\t\x12\x1d\n\x15skip_dependent_tables\x18\x03 \x01(\x08\x12\x1b\n\x13\x64\x65terministic_cq_id\x18\x04 \x01(\x08\x12:\n\x07\x62\x61\x63kend\x18\x05 \x01(\x0b\x32).cloudquery.plugin.v3.Sync.BackendOptions\x1a\x9a\x01\n\x08Response\x12G\n\rmigrate_table\x18\x01 \x01(\x0b\x32..cloudquery.plugin.v3.Sync.MessageMigrateTableH\x00\x12:\n\x06insert\x18\x02 \x01(\x0b\x32(.cloudquery.plugin.v3.Sync.MessageInsertH\x00\x42\t\n\x07message\"<\n\x04Read\x1a\x18\n\x07Request\x12\r\n\x05table\x18\x01 \x01(\x0c\x1a\x1a\n\x08Response\x12\x0e\n\x06record\x18\x01 \x01(\x0c\"\xd2\x03\n\x05Write\x1a;\n\x13MessageMigrateTable\x12\r\n\x05table\x18\x01 \x01(\x0c\x12\x15\n\rmigrate_force\x18\x02 \x01(\x08\x1a\x1f\n\rMessageInsert\x12\x0e\n\x06record\x18\x01 \x01(\x0c\x1a\x7f\n\x12MessageDeleteStale\x12\x11\n\x05table\x18\x01 \x01(\x0c\x42\x02\x18\x01\x12\x13\n\x0bsource_name\x18\x02 \x01(\t\x12-\n\tsync_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ntable_name\x18\x04 \x01(\t\x1a\xdd\x01\n\x07Request\x12H\n\rmigrate_table\x18\x01 \x01(\x0b\x32/.cloudquery.plugin.v3.Write.MessageMigrateTableH\x00\x12;\n\x06insert\x18\x02 \x01(\x0b\x32).cloudquery.plugin.v3.Write.MessageInsertH\x00\x12@\n\x06\x64\x65lete\x18\x03 \x01(\x0b\x32..cloudquery.plugin.v3.Write.MessageDeleteStaleH\x00\x42\t\n\x07message\x1a\n\n\x08Response\"\x1e\n\x05\x43lose\x1a\t\n\x07Request\x1a\n\n\x08Response2\xc6\x05\n\x06Plugin\x12X\n\x07GetName\x12%.cloudquery.plugin.v3.GetName.Request\x1a&.cloudquery.plugin.v3.GetName.Response\x12\x61\n\nGetVersion\x12(.cloudquery.plugin.v3.GetVersion.Request\x1a).cloudquery.plugin.v3.GetVersion.Response\x12O\n\x04Init\x12\".cloudquery.plugin.v3.Init.Request\x1a#.cloudquery.plugin.v3.Init.Response\x12^\n\tGetTables\x12\'.cloudquery.plugin.v3.GetTables.Request\x1a(.cloudquery.plugin.v3.GetTables.Response\x12Q\n\x04Sync\x12\".cloudquery.plugin.v3.Sync.Request\x1a#.cloudquery.plugin.v3.Sync.Response0\x01\x12Q\n\x04Read\x12\".cloudquery.plugin.v3.Read.Request\x1a#.cloudquery.plugin.v3.Read.Response0\x01\x12T\n\x05Write\x12#.cloudquery.plugin.v3.Write.Request\x1a$.cloudquery.plugin.v3.Write.Response(\x01\x12R\n\x05\x43lose\x12#.cloudquery.plugin.v3.Close.Request\x1a$.cloudquery.plugin.v3.Close.ResponseB8Z6github.com/cloudquery/plugin-pb-go/pb/plugin/v3;pluginb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!cloudquery/plugin_v3/plugin.proto\x12\x14\x63loudquery.plugin.v3\x1a\x1fgoogle/protobuf/timestamp.proto\".\n\x07GetName\x1a\t\n\x07Request\x1a\x18\n\x08Response\x12\x0c\n\x04name\x18\x01 \x01(\t\"4\n\nGetVersion\x1a\t\n\x07Request\x1a\x1b\n\x08Response\x12\x0f\n\x07version\x18\x01 \x01(\t\"B\n\x04Init\x1a.\n\x07Request\x12\x0c\n\x04spec\x18\x01 \x01(\x0c\x12\x15\n\rno_connection\x18\x02 \x01(\x08\x1a\n\n\x08Response\"v\n\tGetTables\x1aM\n\x07Request\x12\x0e\n\x06tables\x18\x01 \x03(\t\x12\x13\n\x0bskip_tables\x18\x02 \x03(\t\x12\x1d\n\x15skip_dependent_tables\x18\x03 \x01(\x08\x1a\x1a\n\x08Response\x12\x0e\n\x06tables\x18\x01 \x03(\x0c\"\xcd\x03\n\x04Sync\x1a\x1f\n\rMessageInsert\x12\x0e\n\x06record\x18\x01 \x01(\x0c\x1a$\n\x13MessageMigrateTable\x12\r\n\x05table\x18\x01 \x01(\x0c\x1a\x38\n\x0e\x42\x61\x63kendOptions\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x12\n\nconnection\x18\x02 \x01(\t\x1a\xa6\x01\n\x07Request\x12\x0e\n\x06tables\x18\x01 \x03(\t\x12\x13\n\x0bskip_tables\x18\x02 \x03(\t\x12\x1d\n\x15skip_dependent_tables\x18\x03 \x01(\x08\x12\x1b\n\x13\x64\x65terministic_cq_id\x18\x04 \x01(\x08\x12:\n\x07\x62\x61\x63kend\x18\x05 \x01(\x0b\x32).cloudquery.plugin.v3.Sync.BackendOptions\x1a\x9a\x01\n\x08Response\x12G\n\rmigrate_table\x18\x01 \x01(\x0b\x32..cloudquery.plugin.v3.Sync.MessageMigrateTableH\x00\x12:\n\x06insert\x18\x02 \x01(\x0b\x32(.cloudquery.plugin.v3.Sync.MessageInsertH\x00\x42\t\n\x07message\"<\n\x04Read\x1a\x18\n\x07Request\x12\r\n\x05table\x18\x01 \x01(\x0c\x1a\x1a\n\x08Response\x12\x0e\n\x06record\x18\x01 \x01(\x0c\"\xd2\x03\n\x05Write\x1a;\n\x13MessageMigrateTable\x12\r\n\x05table\x18\x01 \x01(\x0c\x12\x15\n\rmigrate_force\x18\x02 \x01(\x08\x1a\x1f\n\rMessageInsert\x12\x0e\n\x06record\x18\x01 \x01(\x0c\x1a\x7f\n\x12MessageDeleteStale\x12\x11\n\x05table\x18\x01 \x01(\x0c\x42\x02\x18\x01\x12\x13\n\x0bsource_name\x18\x02 \x01(\t\x12-\n\tsync_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ntable_name\x18\x04 \x01(\t\x1a\xdd\x01\n\x07Request\x12H\n\rmigrate_table\x18\x01 \x01(\x0b\x32/.cloudquery.plugin.v3.Write.MessageMigrateTableH\x00\x12;\n\x06insert\x18\x02 \x01(\x0b\x32).cloudquery.plugin.v3.Write.MessageInsertH\x00\x12@\n\x06\x64\x65lete\x18\x03 \x01(\x0b\x32..cloudquery.plugin.v3.Write.MessageDeleteStaleH\x00\x42\t\n\x07message\x1a\n\n\x08Response\"\x1e\n\x05\x43lose\x1a\t\n\x07Request\x1a\n\n\x08Response2\xc6\x05\n\x06Plugin\x12X\n\x07GetName\x12%.cloudquery.plugin.v3.GetName.Request\x1a&.cloudquery.plugin.v3.GetName.Response\x12\x61\n\nGetVersion\x12(.cloudquery.plugin.v3.GetVersion.Request\x1a).cloudquery.plugin.v3.GetVersion.Response\x12O\n\x04Init\x12\".cloudquery.plugin.v3.Init.Request\x1a#.cloudquery.plugin.v3.Init.Response\x12^\n\tGetTables\x12\'.cloudquery.plugin.v3.GetTables.Request\x1a(.cloudquery.plugin.v3.GetTables.Response\x12Q\n\x04Sync\x12\".cloudquery.plugin.v3.Sync.Request\x1a#.cloudquery.plugin.v3.Sync.Response0\x01\x12Q\n\x04Read\x12\".cloudquery.plugin.v3.Read.Request\x1a#.cloudquery.plugin.v3.Read.Response0\x01\x12T\n\x05Write\x12#.cloudquery.plugin.v3.Write.Request\x1a$.cloudquery.plugin.v3.Write.Response(\x01\x12R\n\x05\x43lose\x12#.cloudquery.plugin.v3.Close.Request\x1a$.cloudquery.plugin.v3.Close.ResponseBS\n\x17io.cloudquery.plugin.v3P\x01Z6github.com/cloudquery/plugin-pb-go/pb/plugin/v3;pluginb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'cloudquery.plugin_v3.plugin_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z6github.com/cloudquery/plugin-pb-go/pb/plugin/v3;plugin'
+  DESCRIPTOR._serialized_options = b'\n\027io.cloudquery.plugin.v3P\001Z6github.com/cloudquery/plugin-pb-go/pb/plugin/v3;plugin'
   _WRITE_MESSAGEDELETESTALE.fields_by_name['table']._options = None
   _WRITE_MESSAGEDELETESTALE.fields_by_name['table']._serialized_options = b'\030\001'
   _globals['_GETNAME']._serialized_start=92
   _globals['_GETNAME']._serialized_end=138
   _globals['_GETNAME_REQUEST']._serialized_start=103
   _globals['_GETNAME_REQUEST']._serialized_end=112
   _globals['_GETNAME_RESPONSE']._serialized_start=114
@@ -40,51 +40,51 @@
   _globals['_INIT']._serialized_start=194
   _globals['_INIT']._serialized_end=260
   _globals['_INIT_REQUEST']._serialized_start=202
   _globals['_INIT_REQUEST']._serialized_end=248
   _globals['_INIT_RESPONSE']._serialized_start=114
   _globals['_INIT_RESPONSE']._serialized_end=124
   _globals['_GETTABLES']._serialized_start=262
-  _globals['_GETTABLES']._serialized_end=349
+  _globals['_GETTABLES']._serialized_end=380
   _globals['_GETTABLES_REQUEST']._serialized_start=275
-  _globals['_GETTABLES_REQUEST']._serialized_end=321
-  _globals['_GETTABLES_RESPONSE']._serialized_start=323
-  _globals['_GETTABLES_RESPONSE']._serialized_end=349
-  _globals['_SYNC']._serialized_start=352
-  _globals['_SYNC']._serialized_end=813
-  _globals['_SYNC_MESSAGEINSERT']._serialized_start=360
-  _globals['_SYNC_MESSAGEINSERT']._serialized_end=391
-  _globals['_SYNC_MESSAGEMIGRATETABLE']._serialized_start=393
-  _globals['_SYNC_MESSAGEMIGRATETABLE']._serialized_end=429
-  _globals['_SYNC_BACKENDOPTIONS']._serialized_start=431
-  _globals['_SYNC_BACKENDOPTIONS']._serialized_end=487
-  _globals['_SYNC_REQUEST']._serialized_start=490
-  _globals['_SYNC_REQUEST']._serialized_end=656
-  _globals['_SYNC_RESPONSE']._serialized_start=659
-  _globals['_SYNC_RESPONSE']._serialized_end=813
-  _globals['_READ']._serialized_start=815
-  _globals['_READ']._serialized_end=875
-  _globals['_READ_REQUEST']._serialized_start=823
-  _globals['_READ_REQUEST']._serialized_end=847
-  _globals['_READ_RESPONSE']._serialized_start=849
-  _globals['_READ_RESPONSE']._serialized_end=875
-  _globals['_WRITE']._serialized_start=878
-  _globals['_WRITE']._serialized_end=1344
-  _globals['_WRITE_MESSAGEMIGRATETABLE']._serialized_start=887
-  _globals['_WRITE_MESSAGEMIGRATETABLE']._serialized_end=946
-  _globals['_WRITE_MESSAGEINSERT']._serialized_start=360
-  _globals['_WRITE_MESSAGEINSERT']._serialized_end=391
-  _globals['_WRITE_MESSAGEDELETESTALE']._serialized_start=981
-  _globals['_WRITE_MESSAGEDELETESTALE']._serialized_end=1108
-  _globals['_WRITE_REQUEST']._serialized_start=1111
-  _globals['_WRITE_REQUEST']._serialized_end=1332
+  _globals['_GETTABLES_REQUEST']._serialized_end=352
+  _globals['_GETTABLES_RESPONSE']._serialized_start=354
+  _globals['_GETTABLES_RESPONSE']._serialized_end=380
+  _globals['_SYNC']._serialized_start=383
+  _globals['_SYNC']._serialized_end=844
+  _globals['_SYNC_MESSAGEINSERT']._serialized_start=391
+  _globals['_SYNC_MESSAGEINSERT']._serialized_end=422
+  _globals['_SYNC_MESSAGEMIGRATETABLE']._serialized_start=424
+  _globals['_SYNC_MESSAGEMIGRATETABLE']._serialized_end=460
+  _globals['_SYNC_BACKENDOPTIONS']._serialized_start=462
+  _globals['_SYNC_BACKENDOPTIONS']._serialized_end=518
+  _globals['_SYNC_REQUEST']._serialized_start=521
+  _globals['_SYNC_REQUEST']._serialized_end=687
+  _globals['_SYNC_RESPONSE']._serialized_start=690
+  _globals['_SYNC_RESPONSE']._serialized_end=844
+  _globals['_READ']._serialized_start=846
+  _globals['_READ']._serialized_end=906
+  _globals['_READ_REQUEST']._serialized_start=854
+  _globals['_READ_REQUEST']._serialized_end=878
+  _globals['_READ_RESPONSE']._serialized_start=880
+  _globals['_READ_RESPONSE']._serialized_end=906
+  _globals['_WRITE']._serialized_start=909
+  _globals['_WRITE']._serialized_end=1375
+  _globals['_WRITE_MESSAGEMIGRATETABLE']._serialized_start=918
+  _globals['_WRITE_MESSAGEMIGRATETABLE']._serialized_end=977
+  _globals['_WRITE_MESSAGEINSERT']._serialized_start=391
+  _globals['_WRITE_MESSAGEINSERT']._serialized_end=422
+  _globals['_WRITE_MESSAGEDELETESTALE']._serialized_start=1012
+  _globals['_WRITE_MESSAGEDELETESTALE']._serialized_end=1139
+  _globals['_WRITE_REQUEST']._serialized_start=1142
+  _globals['_WRITE_REQUEST']._serialized_end=1363
   _globals['_WRITE_RESPONSE']._serialized_start=114
   _globals['_WRITE_RESPONSE']._serialized_end=124
-  _globals['_CLOSE']._serialized_start=1346
-  _globals['_CLOSE']._serialized_end=1376
+  _globals['_CLOSE']._serialized_start=1377
+  _globals['_CLOSE']._serialized_end=1407
   _globals['_CLOSE_REQUEST']._serialized_start=103
   _globals['_CLOSE_REQUEST']._serialized_end=112
   _globals['_CLOSE_RESPONSE']._serialized_start=114
   _globals['_CLOSE_RESPONSE']._serialized_end=124
-  _globals['_PLUGIN']._serialized_start=1379
-  _globals['_PLUGIN']._serialized_end=2089
+  _globals['_PLUGIN']._serialized_start=1410
+  _globals['_PLUGIN']._serialized_end=2120
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cloudquery-plugin-pb-0.0.14/cloudquery/plugin_v3/plugin_pb2.pyi` & `cloudquery-plugin-pb-0.0.15/cloudquery/plugin_v3/plugin_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,22 @@
         __slots__ = []
         def __init__(self) -> None: ...
     def __init__(self) -> None: ...
 
 class GetTables(_message.Message):
     __slots__ = []
     class Request(_message.Message):
-        __slots__ = ["tables", "skip_tables"]
+        __slots__ = ["tables", "skip_tables", "skip_dependent_tables"]
         TABLES_FIELD_NUMBER: _ClassVar[int]
         SKIP_TABLES_FIELD_NUMBER: _ClassVar[int]
+        SKIP_DEPENDENT_TABLES_FIELD_NUMBER: _ClassVar[int]
         tables: _containers.RepeatedScalarFieldContainer[str]
         skip_tables: _containers.RepeatedScalarFieldContainer[str]
-        def __init__(self, tables: _Optional[_Iterable[str]] = ..., skip_tables: _Optional[_Iterable[str]] = ...) -> None: ...
+        skip_dependent_tables: bool
+        def __init__(self, tables: _Optional[_Iterable[str]] = ..., skip_tables: _Optional[_Iterable[str]] = ..., skip_dependent_tables: bool = ...) -> None: ...
     class Response(_message.Message):
         __slots__ = ["tables"]
         TABLES_FIELD_NUMBER: _ClassVar[int]
         tables: _containers.RepeatedScalarFieldContainer[bytes]
         def __init__(self, tables: _Optional[_Iterable[bytes]] = ...) -> None: ...
     def __init__(self) -> None: ...
```

### Comparing `cloudquery-plugin-pb-0.0.14/cloudquery/plugin_v3/plugin_pb2_grpc.py` & `cloudquery-plugin-pb-0.0.15/cloudquery/plugin_v3/plugin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.14/cloudquery_plugin_pb.egg-info/PKG-INFO` & `cloudquery-plugin-pb-0.0.15/cloudquery_plugin_pb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-pb
-Version: 0.0.14
+Version: 0.0.15
 Summary: CloudQuery Plugin client and server library
 Home-page: https://github.com/cloudquery/plugin-pb-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-pb-0.0.14/cloudquery_plugin_pb.egg-info/SOURCES.txt` & `cloudquery-plugin-pb-0.0.15/cloudquery_plugin_pb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.14/setup.py` & `cloudquery-plugin-pb-0.0.15/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 description = "CloudQuery Plugin client and server library"
 
 dependencies = [
     "grpcio >= 1.56.0",
     "grpcio-tools >= 1.56.0",
     "protobuf >= 4.23.4",
-    "pyarrow >= 12.0.1"
+    "pyarrow >= 12.0.1",
 ]
 url = "https://github.com/cloudquery/plugin-pb-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 long_description = """
 Python Low Level Client for CloudQuery Plugin
@@ -33,15 +33,15 @@
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("cloudquery")
 ]
 setuptools.setup(
     name=name,
-    version="0.0.14",
+    version="0.0.15",
     description=description,
     long_description=long_description,
     author="CloudQuery LTD",
     author_email="pypi-packages@cloudquery.io",
     license="MPL-2.0",
     url=url,
     classifiers=[
@@ -61,10 +61,17 @@
     platforms="Posix; MacOS X; Windows",
     packages=packages,
     python_requires=">=3.7",
     namespace_packages=["cloudquery"],
     # namespace_packages=namespaces,
     install_requires=dependencies,
     include_package_data=True,
-    package_data={"cloudquery": ["plugin_v3/py.typed", "plugin_v3/*.pyi", "discovery_v1/py.typed", "discovery_v1/*.pyi"]},
+    package_data={
+        "cloudquery": [
+            "plugin_v3/py.typed",
+            "plugin_v3/*.pyi",
+            "discovery_v1/py.typed",
+            "discovery_v1/*.pyi",
+        ]
+    },
     zip_safe=False,
 )
```

