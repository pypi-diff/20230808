# Comparing `tmp/th2_grpc_lw_data_provider-2.0.0.dev5795109852.tar.gz` & `tmp/th2_grpc_lw_data_provider-2.1.0.dev3871883101.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_lw_data_provider-2.0.0.dev5795109852.tar", last modified: Tue Aug  8 09:21:50 2023, max compression
+gzip compressed data, was "dist/th2_grpc_lw_data_provider-2.1.0.dev3871883101.tar", last modified: Mon Jan  9 08:11:56 2023, max compression
```

## Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852.tar` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-08 09:19:54.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-08-08 09:19:54.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4495 2023-08-08 09:19:54.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-08-08 09:21:22.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/data_provider_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     8186 2023-08-08 09:19:54.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/lw_data_provider.proto
--rw-r--r--   0 runner    (1001) docker     (122)    11021 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/lw_data_provider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    30588 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/lw_data_provider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    15651 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/lw_data_provider_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-08-08 09:19:54.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/queue_data_provider.proto
--rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/queue_data_provider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/queue_data_provider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     5036 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/queue_data_provider_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-08-08 09:21:22.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/queue_data_provider_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-08 09:21:50.000000 th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-01-09 08:10:33.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-01-09 08:10:35.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4533 2023-01-09 08:10:33.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-01-09 08:11:34.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/data_provider_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7602 2023-01-09 08:10:33.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/lw_data_provider.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     9528 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/lw_data_provider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26269 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/lw_data_provider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    13839 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/lw_data_provider_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-01-09 08:10:33.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/queue_data_provider.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/queue_data_provider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/queue_data_provider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     5036 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/queue_data_provider_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-01-09 08:11:34.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/queue_data_provider_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-01-09 08:11:56.000000 th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider.egg-info/top_level.txt
```

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/setup.py` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     def initialize_options(self):
         self.strict_mode = False
 
     def finalize_options(self):
         pass
 
     def run(self):
-        proto_path = os.path.abspath('proto')
-        gen_path = os.path.abspath('build/generated/source/proto/main/services/python')
+        proto_path = os.path.abspath('src/main/proto')
+        gen_path = os.path.abspath('src/gen/main/python')
 
         if not os.path.exists(gen_path):
             os.makedirs(gen_path)
 
         proto_files = []
         for root, _, files in os.walk(proto_path):
             for filename in files:
@@ -66,17 +66,18 @@
                 if self.strict_mode:
                     raise Exception(f'error: {command} failed')
 
 
 class CustomDist(sdist):
 
     def run(self):
-        copy_tree(f'proto/{package_name}', package_name)
+        copy_tree(f'src/main/proto/{package_name}', package_name)
 
-        copy_tree(f'build/generated/source/proto/main/services/python/{package_name}', package_name)
+        copy_tree(f'src/gen/main/python/{package_name}', package_name)
+        copy_tree(f'src/gen/main/services/python/{package_name}', package_name)
         Path(f'{package_name}/__init__.py').touch()
         Path(f'{package_name}/py.typed').touch()
 
         def make_packages(root_dir):
             for path in Path(root_dir).iterdir():
                 if path.is_dir():
                     path.joinpath('__init__.py').touch()
```

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/data_provider_service.py` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/data_provider_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,8 @@
     def SearchEvents(self, request, timeout=None, properties=None):
         return self.connector.create_request('SearchEvents', request, timeout, properties)
 
     def SearchMessageGroups(self, request, timeout=None, properties=None):
         return self.connector.create_request('SearchMessageGroups', request, timeout, properties)
 
     def GetBooks(self, request, timeout=None, properties=None):
-        return self.connector.create_request('GetBooks', request, timeout, properties)
-
-    def GetPageInfo(self, request, timeout=None, properties=None):
-        return self.connector.create_request('GetPageInfo', request, timeout, properties)
+        return self.connector.create_request('GetBooks', request, timeout, properties)
```

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/lw_data_provider.proto` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/lw_data_provider.proto`

 * *Files 11% similar despite different names*

```diff
@@ -1,225 +1,200 @@
-/*
- * Copyright 2020-2023 Exactpro (Exactpro Systems Limited)
- *
- * Licensed under the Apache License, Version 2.0 (the "License");
- * you may not use this file except in compliance with the License.
- * You may obtain a copy of the License at
- *
- *     http://www.apache.org/licenses/LICENSE-2.0
- *
- * Unless required by applicable law or agreed to in writing, software
- * distributed under the License is distributed on an "AS IS" BASIS,
- * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
- * See the License for the specific language governing permissions and
- * limitations under the License.
- */
-
-syntax = "proto3";
-
-package th2.data_provider.lw;
-
-import "th2_grpc_common/common.proto";
-import "google/protobuf/timestamp.proto";
-import "google/protobuf/any.proto";
-import "google/protobuf/wrappers.proto";
-
-option java_multiple_files = true;
-option java_package = "com.exactpro.th2.dataprovider.lw.grpc";
-
-
-service DataProvider {
-
-  /* returns a single event with the specified id */
-  rpc GetEvent (EventID) returns (EventResponse);
-
-  /* returns a single message with the specified id */
-  rpc GetMessage (MessageID) returns (MessageGroupResponse);
-
-  /* returns a list of message stream names */
-  rpc GetMessageStreams (MessageStreamsRequest) returns (MessageStreamsResponse);
-
-  /* creates a message stream that matches the filter. */
-  rpc SearchMessages (MessageSearchRequest) returns (stream MessageSearchResponse);
-
-  /* creates an event or an event metadata stream that matches the filter. */
-  rpc SearchEvents (EventSearchRequest) returns (stream EventSearchResponse);
-
-  /*
-  Searches for messages groups in specified timestamp
-   */
-  rpc SearchMessageGroups (MessageGroupsSearchRequest) returns (stream MessageSearchResponse);
-
-  // Returns the set of books stored in cradle cache
-  rpc GetBooks(BooksRequest) returns (BooksResponse);
-
-  rpc GetPageInfo(PageInfoRequest) returns (stream PageInfoResponse);
-}
-
-// The scope for events to request
-message EventScope {
-  string name = 1;
-}
-
-message BookId {
-  // Name of the book to request data from
-  string name = 1;
-}
-
-message MessageGroupsSearchRequest {
-  message Group {
-    string name = 1;
-  }
-  google.protobuf.Timestamp start_timestamp = 1;
-  google.protobuf.Timestamp end_timestamp = 2;
-  BookId book_id = 7;
-  repeated Group message_group = 3;
-  google.protobuf.BoolValue sort = 4;
-  // deprecated: use response_formats with only BASE_64 to achieve the same effect
-  bool raw_only = 5 [deprecated = true];
-  bool keep_open = 6;
-  repeated string response_formats = 8; // List of possible response formats (e.g. PARSED or BASE_64)
-}
-
-message MessageStreamsRequest {
-  BookId book_id = 1;
-}
-
-message EventResponse {
-  EventID event_id = 1; // Current event id
-  EventID parent_event_id = 2; // Event id of a parent event. It is absent for root event
-
-  EventID batch_id = 3; // Event id of a parent event. It is absent for root event
-
-  bool is_batched = 4; // Flag indicating that the event is in batch
-
-  google.protobuf.Timestamp start_timestamp = 5;
-  google.protobuf.Timestamp end_timestamp = 6; // May be absent.
-  EventStatus status = 7; // Aggregated status of current and children events which sync written.
-  string event_name = 8;
-  string event_type = 9; // May be absent.
-  bytes body = 10; // May be absent.
-  repeated MessageID attached_message_id = 11; // ids of messages linked to this event
-}
-
-message MessageGroupItem {
-  Message message = 1;
-  bool match = 2;
-}
-
-message MessageGroupResponse {
-  MessageID message_id = 1; // Message id should be unique in session
-  google.protobuf.Timestamp timestamp = 2 [deprecated = true]; // Message creation timestamp. Deprecated. Moved to MessageID
-  map<string, string> message_properties = 6; // Additional properties for the source raw message
-  bytes body_raw = 3;
-  repeated EventID attached_event_id = 4; // ids of events linked to this message group
-  repeated MessageGroupItem message_item = 5; // May be absent.
-}
-
-message FilterName {
-  string name = 1;
-}
-
-message Filter {
-  FilterName name = 1;
-  bool negative = 2;
-  repeated string value = 3;
-  bool conjunct = 4;
-}
-
-message EventSearchRequest {
-  google.protobuf.Timestamp start_timestamp = 1; // unix timestamp - Sets the search starting point. One of the 'start_timestamp' or 'resume_from_id' must not absent
-  google.protobuf.Timestamp end_timestamp = 2; // unix timestamp - Sets the timestamp to which the search will be performed, starting with 'start_timestamp'. When 'search_direction' is previous, end_timestamp must be less than start_timestamp. By default it is absent (the search is carried out endlessly into the past or into the future).
-
-  EventID parent_event = 3; // Match events to the specified parent. Only the immediate children of the specified event will be returned.
-  TimeRelation search_direction = 4; // Sets the lookup direction. Can be used for pagination. Set by default to NEXT.
-
-  google.protobuf.Int32Value result_count_limit = 5; // Sets the maximum amount of events to return. By default it is absent (unlimited).
-
-  repeated Filter filter = 6; // List of event search filters. (See 'search/sse/events' HTTP method https://github.com/th2-net/th2-rpt-data-provider)
-
-  BookId book_id = 7;
-  EventScope scope = 8;
-}
-
-message EventSearchResponse {
-  oneof data {
-    EventResponse event = 1;
-  }
-}
-
-message MessageSearchRequest {
-  google.protobuf.Timestamp start_timestamp = 1; // unix timestamp - Sets the search starting point. One of the 'start_timestamp' or 'resume_from_id' or 'message_id' must not absent
-  google.protobuf.Timestamp end_timestamp = 2; // unix timestamp - Sets the timestamp to which the search will be performed, starting with 'start_timestamp'. When search_direction is 'previous', 'end_timestamp' must be less than 'start_timestamp'. By default it is absent (the search is carried out endlessly into the past or into the future).
-
-  TimeRelation search_direction = 3; // Sets the lookup direction. Can be used for pagination. Set by default to NEXT.
-
-  google.protobuf.Int32Value result_count_limit = 4; // Sets the maximum amount of messages to return. By default it is absent (unlimited)
-
-  repeated MessageStream stream = 5; // Sets the stream names and directions to search in. Case-sensitive. Required.
-  google.protobuf.BoolValue keep_open = 6; //  If the search has reached the current moment, it is necessary to wait further for the appearance of new data. Set by default to false.
-
-  repeated MessageStreamPointer stream_pointer = 7; // List of stream pointers to restore the search from. start_timestamp will be ignored if this parameter is specified. By default it is absent.
-
-  repeated string response_formats = 8; // List of possible response formats (e.g. PARSED or BASE_64)
-  BookId book_id = 9;
-}
-
-message MessageSearchResponse {
-  oneof data {
-    MessageGroupResponse message = 1;
-    MessageStreamPointers message_stream_pointers = 2;
-  }
-}
-
-message MessageStreamPointers {
-  repeated MessageStreamPointer message_stream_pointer = 1;
-}
-
-/* This object contains the data of the last message in the stream on which
- * the search has stopped, it is necessary to continue the search from the same point */
- message MessageStreamPointer {
-  MessageStream message_stream = 1;
-  MessageID last_id = 2; // Might be absent if the stream has no messages
-}
-
-message MessageStream {
-  string name = 1; // Case sensitive. Required.
-  Direction direction = 2; // Required.
-}
-
-message MessageStreamsResponse {
-  repeated MessageStream message_stream = 1;
-}
-
-enum TimeRelation {
-  NEXT = 0;
-  PREVIOUS = 1;
-}
-
-message BooksRequest {
-}
-
-message BooksResponse {
-  repeated BookId book_ids = 1;
-}
-
-message PageInfoRequest {
-  BookId book_id = 1;
-  google.protobuf.Timestamp start_timestamp = 2;
-  google.protobuf.Timestamp end_timestamp = 3;
-  google.protobuf.Int32Value result_limit = 4;
-}
-
-message PageInfoResponse {
-  PageId id = 1;
-  google.protobuf.StringValue comment = 2;
-  google.protobuf.Timestamp started = 3;
-  google.protobuf.Timestamp ended = 4;
-  google.protobuf.Timestamp updated = 5;
-  google.protobuf.Timestamp removed = 6;
-}
-
-message PageId {
-  BookId book_id = 1;
-  string name = 2;
+/*
+ * Copyright 2020-2020 Exactpro (Exactpro Systems Limited)
+ *
+ * Licensed under the Apache License, Version 2.0 (the "License");
+ * you may not use this file except in compliance with the License.
+ * You may obtain a copy of the License at
+ *
+ *     http://www.apache.org/licenses/LICENSE-2.0
+ *
+ * Unless required by applicable law or agreed to in writing, software
+ * distributed under the License is distributed on an "AS IS" BASIS,
+ * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+ * See the License for the specific language governing permissions and
+ * limitations under the License.
+ */
+
+syntax = "proto3";
+
+package th2.data_provider.lw;
+
+import "th2_grpc_common/common.proto";
+import "google/protobuf/timestamp.proto";
+import "google/protobuf/any.proto";
+import "google/protobuf/wrappers.proto";
+
+option java_multiple_files = true;
+option java_package = "com.exactpro.th2.dataprovider.lw.grpc";
+
+
+service DataProvider {
+
+  /* returns a single event with the specified id */
+  rpc GetEvent (EventID) returns (EventResponse);
+
+  /* returns a single message with the specified id */
+  rpc GetMessage (MessageID) returns (MessageGroupResponse);
+
+  /* returns a list of message stream names */
+  rpc GetMessageStreams (MessageStreamsRequest) returns (MessageStreamsResponse);
+
+  /* creates a message stream that matches the filter. */
+  rpc SearchMessages (MessageSearchRequest) returns (stream MessageSearchResponse);
+
+  /* creates an event or an event metadata stream that matches the filter. */
+  rpc SearchEvents (EventSearchRequest) returns (stream EventSearchResponse);
+
+  /*
+  Searches for messages groups in specified timestamp
+   */
+  rpc SearchMessageGroups (MessageGroupsSearchRequest) returns (stream MessageSearchResponse);
+
+  // Returns the set of books stored in cradle cache
+  rpc GetBooks(BooksRequest) returns (BooksResponse);
+}
+
+// The scope for events to request
+message EventScope {
+  string name = 1;
+}
+
+message BookId {
+  // Name of the book to request data from
+  string name = 1;
+}
+
+message MessageGroupsSearchRequest {
+  message Group {
+    string name = 1;
+  }
+  google.protobuf.Timestamp start_timestamp = 1;
+  google.protobuf.Timestamp end_timestamp = 2;
+  BookId book_id = 7;
+  repeated Group message_group = 3;
+  google.protobuf.BoolValue sort = 4;
+  bool raw_only = 5;
+  bool keep_open = 6;
+}
+
+message MessageStreamsRequest {
+  BookId book_id = 1;
+}
+
+message EventResponse {
+  EventID event_id = 1; // Current event id
+  EventID parent_event_id = 2; // Event id of a parent event. It is absent for root event
+
+  EventID batch_id = 3; // Event id of a parent event. It is absent for root event
+
+  bool is_batched = 4; // Flag indicating that the event is in batch
+
+  google.protobuf.Timestamp start_timestamp = 5;
+  google.protobuf.Timestamp end_timestamp = 6; // May be absent.
+  EventStatus status = 7; // Aggregated status of current and children events which sync written.
+  string event_name = 8;
+  string event_type = 9; // May be absent.
+  bytes body = 10; // May be absent.
+  repeated MessageID attached_message_id = 11; // ids of messages linked to this event
+}
+
+message MessageGroupItem {
+  Message message = 1;
+  bool match = 2;
+}
+
+message MessageGroupResponse {
+  MessageID message_id = 1; // Message id should be unique in session
+  google.protobuf.Timestamp timestamp = 2 [deprecated = true]; // Message creation timestamp. Deprecated. Moved to MessageID
+  map<string, string> message_properties = 6; // Additional properties for the source raw message
+  bytes body_raw = 3;
+  repeated EventID attached_event_id = 4; // ids of events linked to this message group
+  repeated MessageGroupItem message_item = 5; // May be absent.
+}
+
+message FilterName {
+  string name = 1;
+}
+
+message Filter {
+  FilterName name = 1;
+  bool negative = 2;
+  repeated string value = 3;
+  bool conjunct = 4;
+}
+
+message EventSearchRequest {
+  google.protobuf.Timestamp start_timestamp = 1; // unix timestamp - Sets the search starting point. One of the 'start_timestamp' or 'resume_from_id' must not absent
+  google.protobuf.Timestamp end_timestamp = 2; // unix timestamp - Sets the timestamp to which the search will be performed, starting with 'start_timestamp'. When 'search_direction' is previous, end_timestamp must be less than start_timestamp. By default it is absent (the search is carried out endlessly into the past or into the future).
+
+  EventID parent_event = 3; // Match events to the specified parent. Only the immediate children of the specified event will be returned.
+  TimeRelation search_direction = 4; // Sets the lookup direction. Can be used for pagination. Set by default to NEXT.
+
+  google.protobuf.Int32Value result_count_limit = 5; // Sets the maximum amount of events to return. By default it is absent (unlimited).
+
+  repeated Filter filter = 6; // List of event search filters. (See 'search/sse/events' HTTP method https://github.com/th2-net/th2-rpt-data-provider)
+
+  BookId book_id = 7;
+  EventScope scope = 8;
+}
+
+message EventSearchResponse {
+  oneof data {
+    EventResponse event = 1;
+  }
+}
+
+message MessageSearchRequest {
+  google.protobuf.Timestamp start_timestamp = 1; // unix timestamp - Sets the search starting point. One of the 'start_timestamp' or 'resume_from_id' or 'message_id' must not absent
+  google.protobuf.Timestamp end_timestamp = 2; // unix timestamp - Sets the timestamp to which the search will be performed, starting with 'start_timestamp'. When search_direction is 'previous', 'end_timestamp' must be less than 'start_timestamp'. By default it is absent (the search is carried out endlessly into the past or into the future).
+
+  TimeRelation search_direction = 3; // Sets the lookup direction. Can be used for pagination. Set by default to NEXT.
+
+  google.protobuf.Int32Value result_count_limit = 4; // Sets the maximum amount of messages to return. By default it is absent (unlimited)
+
+  repeated MessageStream stream = 5; // Sets the stream names and directions to search in. Case-sensitive. Required.
+  google.protobuf.BoolValue keep_open = 6; //  If the search has reached the current moment, it is necessary to wait further for the appearance of new data. Set by default to false.
+
+  repeated MessageStreamPointer stream_pointer = 7; // List of stream pointers to restore the search from. start_timestamp will be ignored if this parameter is specified. By default it is absent.
+
+  repeated string response_formats = 8; // List of possible response formats (e.g. PARSED or BASE_64)
+  BookId book_id = 9;
+}
+
+message MessageSearchResponse {
+  oneof data {
+    MessageGroupResponse message = 1;
+    MessageStreamPointers message_stream_pointers = 2;
+  }
+}
+
+message MessageStreamPointers {
+  repeated MessageStreamPointer message_stream_pointer = 1;
+}
+
+/* This object contains the data of the last message in the stream on which
+ * the search has stopped, it is necessary to continue the search from the same point */
+ message MessageStreamPointer {
+  MessageStream message_stream = 1;
+  MessageID last_id = 2; // Might be absent if the stream has no messages
+}
+
+message MessageStream {
+  string name = 1; // Case sensitive. Required.
+  Direction direction = 2; // Required.
+}
+
+message MessageStreamsResponse {
+  repeated MessageStream message_stream = 1;
+}
+
+enum TimeRelation {
+  NEXT = 0;
+  PREVIOUS = 1;
+}
+
+message BooksRequest {
+}
+
+message BooksResponse {
+  repeated BookId book_ids = 1;
 }
```

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/lw_data_provider_pb2.py` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/lw_data_provider_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,74 +13,66 @@
 
 from th2_grpc_common import common_pb2 as th2__grpc__common_dot_common__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0th2_grpc_lw_data_provider/lw_data_provider.proto\x12\x14th2.data_provider.lw\x1a\x1cth2_grpc_common/common.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x1a\n\nEventScope\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x16\n\x06\x42ookId\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x86\x03\n\x1aMessageGroupsSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x07\x62ook_id\x18\x07 \x01(\x0b\x32\x1c.th2.data_provider.lw.BookId\x12M\n\rmessage_group\x18\x03 \x03(\x0b\x32\x36.th2.data_provider.lw.MessageGroupsSearchRequest.Group\x12(\n\x04sort\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x14\n\x08raw_only\x18\x05 \x01(\x08\x42\x02\x18\x01\x12\x11\n\tkeep_open\x18\x06 \x01(\x08\x12\x18\n\x10response_formats\x18\x08 \x03(\t\x1a\x15\n\x05Group\x12\x0c\n\x04name\x18\x01 \x01(\t\"F\n\x15MessageStreamsRequest\x12-\n\x07\x62ook_id\x18\x01 \x01(\x0b\x32\x1c.th2.data_provider.lw.BookId\"\xe3\x02\n\rEventResponse\x12\x1a\n\x08\x65vent_id\x18\x01 \x01(\x0b\x32\x08.EventID\x12!\n\x0fparent_event_id\x18\x02 \x01(\x0b\x32\x08.EventID\x12\x1a\n\x08\x62\x61tch_id\x18\x03 \x01(\x0b\x32\x08.EventID\x12\x12\n\nis_batched\x18\x04 \x01(\x08\x12\x33\n\x0fstart_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x06status\x18\x07 \x01(\x0e\x32\x0c.EventStatus\x12\x12\n\nevent_name\x18\x08 \x01(\t\x12\x12\n\nevent_type\x18\t \x01(\t\x12\x0c\n\x04\x62ody\x18\n \x01(\x0c\x12\'\n\x13\x61ttached_message_id\x18\x0b \x03(\x0b\x32\n.MessageID\"<\n\x10MessageGroupItem\x12\x19\n\x07message\x18\x01 \x01(\x0b\x32\x08.Message\x12\r\n\x05match\x18\x02 \x01(\x08\"\xf7\x02\n\x14MessageGroupResponse\x12\x1e\n\nmessage_id\x18\x01 \x01(\x0b\x32\n.MessageID\x12\x31\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12]\n\x12message_properties\x18\x06 \x03(\x0b\x32\x41.th2.data_provider.lw.MessageGroupResponse.MessagePropertiesEntry\x12\x10\n\x08\x62ody_raw\x18\x03 \x01(\x0c\x12#\n\x11\x61ttached_event_id\x18\x04 \x03(\x0b\x32\x08.EventID\x12<\n\x0cmessage_item\x18\x05 \x03(\x0b\x32&.th2.data_provider.lw.MessageGroupItem\x1a\x38\n\x16MessagePropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x1a\n\nFilterName\x12\x0c\n\x04name\x18\x01 \x01(\t\"k\n\x06\x46ilter\x12.\n\x04name\x18\x01 \x01(\x0b\x32 .th2.data_provider.lw.FilterName\x12\x10\n\x08negative\x18\x02 \x01(\x08\x12\r\n\x05value\x18\x03 \x03(\t\x12\x10\n\x08\x63onjunct\x18\x04 \x01(\x08\"\xa1\x03\n\x12\x45ventSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x0cparent_event\x18\x03 \x01(\x0b\x32\x08.EventID\x12<\n\x10search_direction\x18\x04 \x01(\x0e\x32\".th2.data_provider.lw.TimeRelation\x12\x37\n\x12result_count_limit\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12,\n\x06\x66ilter\x18\x06 \x03(\x0b\x32\x1c.th2.data_provider.lw.Filter\x12-\n\x07\x62ook_id\x18\x07 \x01(\x0b\x32\x1c.th2.data_provider.lw.BookId\x12/\n\x05scope\x18\x08 \x01(\x0b\x32 .th2.data_provider.lw.EventScope\"S\n\x13\x45ventSearchResponse\x12\x34\n\x05\x65vent\x18\x01 \x01(\x0b\x32#.th2.data_provider.lw.EventResponseH\x00\x42\x06\n\x04\x64\x61ta\"\xe6\x03\n\x14MessageSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12<\n\x10search_direction\x18\x03 \x01(\x0e\x32\".th2.data_provider.lw.TimeRelation\x12\x37\n\x12result_count_limit\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x33\n\x06stream\x18\x05 \x03(\x0b\x32#.th2.data_provider.lw.MessageStream\x12-\n\tkeep_open\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x42\n\x0estream_pointer\x18\x07 \x03(\x0b\x32*.th2.data_provider.lw.MessageStreamPointer\x12\x18\n\x10response_formats\x18\x08 \x03(\t\x12-\n\x07\x62ook_id\x18\t \x01(\x0b\x32\x1c.th2.data_provider.lw.BookId\"\xae\x01\n\x15MessageSearchResponse\x12=\n\x07message\x18\x01 \x01(\x0b\x32*.th2.data_provider.lw.MessageGroupResponseH\x00\x12N\n\x17message_stream_pointers\x18\x02 \x01(\x0b\x32+.th2.data_provider.lw.MessageStreamPointersH\x00\x42\x06\n\x04\x64\x61ta\"c\n\x15MessageStreamPointers\x12J\n\x16message_stream_pointer\x18\x01 \x03(\x0b\x32*.th2.data_provider.lw.MessageStreamPointer\"p\n\x14MessageStreamPointer\x12;\n\x0emessage_stream\x18\x01 \x01(\x0b\x32#.th2.data_provider.lw.MessageStream\x12\x1b\n\x07last_id\x18\x02 \x01(\x0b\x32\n.MessageID\"<\n\rMessageStream\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\tdirection\x18\x02 \x01(\x0e\x32\n.Direction\"U\n\x16MessageStreamsResponse\x12;\n\x0emessage_stream\x18\x01 \x03(\x0b\x32#.th2.data_provider.lw.MessageStream\"\x0e\n\x0c\x42ooksRequest\"?\n\rBooksResponse\x12.\n\x08\x62ook_ids\x18\x01 \x03(\x0b\x32\x1c.th2.data_provider.lw.BookId\"\xdb\x01\n\x0fPageInfoRequest\x12-\n\x07\x62ook_id\x18\x01 \x01(\x0b\x32\x1c.th2.data_provider.lw.BookId\x12\x33\n\x0fstart_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\x0cresult_limit\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\"\x9d\x02\n\x10PageInfoResponse\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.th2.data_provider.lw.PageId\x12-\n\x07\x63omment\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x07started\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x05\x65nded\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07updated\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07removed\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"E\n\x06PageId\x12-\n\x07\x62ook_id\x18\x01 \x01(\x0b\x32\x1c.th2.data_provider.lw.BookId\x12\x0c\n\x04name\x18\x02 \x01(\t*&\n\x0cTimeRelation\x12\x08\n\x04NEXT\x10\x00\x12\x0c\n\x08PREVIOUS\x10\x01\x32\x80\x06\n\x0c\x44\x61taProvider\x12\x39\n\x08GetEvent\x12\x08.EventID\x1a#.th2.data_provider.lw.EventResponse\x12\x44\n\nGetMessage\x12\n.MessageID\x1a*.th2.data_provider.lw.MessageGroupResponse\x12n\n\x11GetMessageStreams\x12+.th2.data_provider.lw.MessageStreamsRequest\x1a,.th2.data_provider.lw.MessageStreamsResponse\x12k\n\x0eSearchMessages\x12*.th2.data_provider.lw.MessageSearchRequest\x1a+.th2.data_provider.lw.MessageSearchResponse0\x01\x12\x65\n\x0cSearchEvents\x12(.th2.data_provider.lw.EventSearchRequest\x1a).th2.data_provider.lw.EventSearchResponse0\x01\x12v\n\x13SearchMessageGroups\x12\x30.th2.data_provider.lw.MessageGroupsSearchRequest\x1a+.th2.data_provider.lw.MessageSearchResponse0\x01\x12S\n\x08GetBooks\x12\".th2.data_provider.lw.BooksRequest\x1a#.th2.data_provider.lw.BooksResponse\x12^\n\x0bGetPageInfo\x12%.th2.data_provider.lw.PageInfoRequest\x1a&.th2.data_provider.lw.PageInfoResponse0\x01\x42)\n%com.exactpro.th2.dataprovider.lw.grpcP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0th2_grpc_lw_data_provider/lw_data_provider.proto\x12\x14th2.data_provider.lw\x1a\x1cth2_grpc_common/common.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x1a\n\nEventScope\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x16\n\x06\x42ookId\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xe8\x02\n\x1aMessageGroupsSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x07\x62ook_id\x18\x07 \x01(\x0b\x32\x1c.th2.data_provider.lw.BookId\x12M\n\rmessage_group\x18\x03 \x03(\x0b\x32\x36.th2.data_provider.lw.MessageGroupsSearchRequest.Group\x12(\n\x04sort\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x10\n\x08raw_only\x18\x05 \x01(\x08\x12\x11\n\tkeep_open\x18\x06 \x01(\x08\x1a\x15\n\x05Group\x12\x0c\n\x04name\x18\x01 \x01(\t\"F\n\x15MessageStreamsRequest\x12-\n\x07\x62ook_id\x18\x01 \x01(\x0b\x32\x1c.th2.data_provider.lw.BookId\"\xe3\x02\n\rEventResponse\x12\x1a\n\x08\x65vent_id\x18\x01 \x01(\x0b\x32\x08.EventID\x12!\n\x0fparent_event_id\x18\x02 \x01(\x0b\x32\x08.EventID\x12\x1a\n\x08\x62\x61tch_id\x18\x03 \x01(\x0b\x32\x08.EventID\x12\x12\n\nis_batched\x18\x04 \x01(\x08\x12\x33\n\x0fstart_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x06status\x18\x07 \x01(\x0e\x32\x0c.EventStatus\x12\x12\n\nevent_name\x18\x08 \x01(\t\x12\x12\n\nevent_type\x18\t \x01(\t\x12\x0c\n\x04\x62ody\x18\n \x01(\x0c\x12\'\n\x13\x61ttached_message_id\x18\x0b \x03(\x0b\x32\n.MessageID\"<\n\x10MessageGroupItem\x12\x19\n\x07message\x18\x01 \x01(\x0b\x32\x08.Message\x12\r\n\x05match\x18\x02 \x01(\x08\"\xf7\x02\n\x14MessageGroupResponse\x12\x1e\n\nmessage_id\x18\x01 \x01(\x0b\x32\n.MessageID\x12\x31\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12]\n\x12message_properties\x18\x06 \x03(\x0b\x32\x41.th2.data_provider.lw.MessageGroupResponse.MessagePropertiesEntry\x12\x10\n\x08\x62ody_raw\x18\x03 \x01(\x0c\x12#\n\x11\x61ttached_event_id\x18\x04 \x03(\x0b\x32\x08.EventID\x12<\n\x0cmessage_item\x18\x05 \x03(\x0b\x32&.th2.data_provider.lw.MessageGroupItem\x1a\x38\n\x16MessagePropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x1a\n\nFilterName\x12\x0c\n\x04name\x18\x01 \x01(\t\"k\n\x06\x46ilter\x12.\n\x04name\x18\x01 \x01(\x0b\x32 .th2.data_provider.lw.FilterName\x12\x10\n\x08negative\x18\x02 \x01(\x08\x12\r\n\x05value\x18\x03 \x03(\t\x12\x10\n\x08\x63onjunct\x18\x04 \x01(\x08\"\xa1\x03\n\x12\x45ventSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x0cparent_event\x18\x03 \x01(\x0b\x32\x08.EventID\x12<\n\x10search_direction\x18\x04 \x01(\x0e\x32\".th2.data_provider.lw.TimeRelation\x12\x37\n\x12result_count_limit\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12,\n\x06\x66ilter\x18\x06 \x03(\x0b\x32\x1c.th2.data_provider.lw.Filter\x12-\n\x07\x62ook_id\x18\x07 \x01(\x0b\x32\x1c.th2.data_provider.lw.BookId\x12/\n\x05scope\x18\x08 \x01(\x0b\x32 .th2.data_provider.lw.EventScope\"S\n\x13\x45ventSearchResponse\x12\x34\n\x05\x65vent\x18\x01 \x01(\x0b\x32#.th2.data_provider.lw.EventResponseH\x00\x42\x06\n\x04\x64\x61ta\"\xe6\x03\n\x14MessageSearchRequest\x12\x33\n\x0fstart_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12<\n\x10search_direction\x18\x03 \x01(\x0e\x32\".th2.data_provider.lw.TimeRelation\x12\x37\n\x12result_count_limit\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x33\n\x06stream\x18\x05 \x03(\x0b\x32#.th2.data_provider.lw.MessageStream\x12-\n\tkeep_open\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x42\n\x0estream_pointer\x18\x07 \x03(\x0b\x32*.th2.data_provider.lw.MessageStreamPointer\x12\x18\n\x10response_formats\x18\x08 \x03(\t\x12-\n\x07\x62ook_id\x18\t \x01(\x0b\x32\x1c.th2.data_provider.lw.BookId\"\xae\x01\n\x15MessageSearchResponse\x12=\n\x07message\x18\x01 \x01(\x0b\x32*.th2.data_provider.lw.MessageGroupResponseH\x00\x12N\n\x17message_stream_pointers\x18\x02 \x01(\x0b\x32+.th2.data_provider.lw.MessageStreamPointersH\x00\x42\x06\n\x04\x64\x61ta\"c\n\x15MessageStreamPointers\x12J\n\x16message_stream_pointer\x18\x01 \x03(\x0b\x32*.th2.data_provider.lw.MessageStreamPointer\"p\n\x14MessageStreamPointer\x12;\n\x0emessage_stream\x18\x01 \x01(\x0b\x32#.th2.data_provider.lw.MessageStream\x12\x1b\n\x07last_id\x18\x02 \x01(\x0b\x32\n.MessageID\"<\n\rMessageStream\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\tdirection\x18\x02 \x01(\x0e\x32\n.Direction\"U\n\x16MessageStreamsResponse\x12;\n\x0emessage_stream\x18\x01 \x03(\x0b\x32#.th2.data_provider.lw.MessageStream\"\x0e\n\x0c\x42ooksRequest\"?\n\rBooksResponse\x12.\n\x08\x62ook_ids\x18\x01 \x03(\x0b\x32\x1c.th2.data_provider.lw.BookId*&\n\x0cTimeRelation\x12\x08\n\x04NEXT\x10\x00\x12\x0c\n\x08PREVIOUS\x10\x01\x32\xa0\x05\n\x0c\x44\x61taProvider\x12\x39\n\x08GetEvent\x12\x08.EventID\x1a#.th2.data_provider.lw.EventResponse\x12\x44\n\nGetMessage\x12\n.MessageID\x1a*.th2.data_provider.lw.MessageGroupResponse\x12n\n\x11GetMessageStreams\x12+.th2.data_provider.lw.MessageStreamsRequest\x1a,.th2.data_provider.lw.MessageStreamsResponse\x12k\n\x0eSearchMessages\x12*.th2.data_provider.lw.MessageSearchRequest\x1a+.th2.data_provider.lw.MessageSearchResponse0\x01\x12\x65\n\x0cSearchEvents\x12(.th2.data_provider.lw.EventSearchRequest\x1a).th2.data_provider.lw.EventSearchResponse0\x01\x12v\n\x13SearchMessageGroups\x12\x30.th2.data_provider.lw.MessageGroupsSearchRequest\x1a+.th2.data_provider.lw.MessageSearchResponse0\x01\x12S\n\x08GetBooks\x12\".th2.data_provider.lw.BooksRequest\x1a#.th2.data_provider.lw.BooksResponseB)\n%com.exactpro.th2.dataprovider.lw.grpcP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'th2_grpc_lw_data_provider.lw_data_provider_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n%com.exactpro.th2.dataprovider.lw.grpcP\001'
-  _MESSAGEGROUPSSEARCHREQUEST.fields_by_name['raw_only']._options = None
-  _MESSAGEGROUPSSEARCHREQUEST.fields_by_name['raw_only']._serialized_options = b'\030\001'
   _MESSAGEGROUPRESPONSE_MESSAGEPROPERTIESENTRY._options = None
   _MESSAGEGROUPRESPONSE_MESSAGEPROPERTIESENTRY._serialized_options = b'8\001'
   _MESSAGEGROUPRESPONSE.fields_by_name['timestamp']._options = None
   _MESSAGEGROUPRESPONSE.fields_by_name['timestamp']._serialized_options = b'\030\001'
-  _TIMERELATION._serialized_start=3845
-  _TIMERELATION._serialized_end=3883
+  _TIMERELATION._serialized_start=3234
+  _TIMERELATION._serialized_end=3272
   _EVENTSCOPE._serialized_start=196
   _EVENTSCOPE._serialized_end=222
   _BOOKID._serialized_start=224
   _BOOKID._serialized_end=246
   _MESSAGEGROUPSSEARCHREQUEST._serialized_start=249
-  _MESSAGEGROUPSSEARCHREQUEST._serialized_end=639
-  _MESSAGEGROUPSSEARCHREQUEST_GROUP._serialized_start=618
-  _MESSAGEGROUPSSEARCHREQUEST_GROUP._serialized_end=639
-  _MESSAGESTREAMSREQUEST._serialized_start=641
-  _MESSAGESTREAMSREQUEST._serialized_end=711
-  _EVENTRESPONSE._serialized_start=714
-  _EVENTRESPONSE._serialized_end=1069
-  _MESSAGEGROUPITEM._serialized_start=1071
-  _MESSAGEGROUPITEM._serialized_end=1131
-  _MESSAGEGROUPRESPONSE._serialized_start=1134
-  _MESSAGEGROUPRESPONSE._serialized_end=1509
-  _MESSAGEGROUPRESPONSE_MESSAGEPROPERTIESENTRY._serialized_start=1453
-  _MESSAGEGROUPRESPONSE_MESSAGEPROPERTIESENTRY._serialized_end=1509
-  _FILTERNAME._serialized_start=1511
-  _FILTERNAME._serialized_end=1537
-  _FILTER._serialized_start=1539
-  _FILTER._serialized_end=1646
-  _EVENTSEARCHREQUEST._serialized_start=1649
-  _EVENTSEARCHREQUEST._serialized_end=2066
-  _EVENTSEARCHRESPONSE._serialized_start=2068
-  _EVENTSEARCHRESPONSE._serialized_end=2151
-  _MESSAGESEARCHREQUEST._serialized_start=2154
-  _MESSAGESEARCHREQUEST._serialized_end=2640
-  _MESSAGESEARCHRESPONSE._serialized_start=2643
-  _MESSAGESEARCHRESPONSE._serialized_end=2817
-  _MESSAGESTREAMPOINTERS._serialized_start=2819
-  _MESSAGESTREAMPOINTERS._serialized_end=2918
-  _MESSAGESTREAMPOINTER._serialized_start=2920
-  _MESSAGESTREAMPOINTER._serialized_end=3032
-  _MESSAGESTREAM._serialized_start=3034
-  _MESSAGESTREAM._serialized_end=3094
-  _MESSAGESTREAMSRESPONSE._serialized_start=3096
-  _MESSAGESTREAMSRESPONSE._serialized_end=3181
-  _BOOKSREQUEST._serialized_start=3183
-  _BOOKSREQUEST._serialized_end=3197
-  _BOOKSRESPONSE._serialized_start=3199
-  _BOOKSRESPONSE._serialized_end=3262
-  _PAGEINFOREQUEST._serialized_start=3265
-  _PAGEINFOREQUEST._serialized_end=3484
-  _PAGEINFORESPONSE._serialized_start=3487
-  _PAGEINFORESPONSE._serialized_end=3772
-  _PAGEID._serialized_start=3774
-  _PAGEID._serialized_end=3843
-  _DATAPROVIDER._serialized_start=3886
-  _DATAPROVIDER._serialized_end=4654
+  _MESSAGEGROUPSSEARCHREQUEST._serialized_end=609
+  _MESSAGEGROUPSSEARCHREQUEST_GROUP._serialized_start=588
+  _MESSAGEGROUPSSEARCHREQUEST_GROUP._serialized_end=609
+  _MESSAGESTREAMSREQUEST._serialized_start=611
+  _MESSAGESTREAMSREQUEST._serialized_end=681
+  _EVENTRESPONSE._serialized_start=684
+  _EVENTRESPONSE._serialized_end=1039
+  _MESSAGEGROUPITEM._serialized_start=1041
+  _MESSAGEGROUPITEM._serialized_end=1101
+  _MESSAGEGROUPRESPONSE._serialized_start=1104
+  _MESSAGEGROUPRESPONSE._serialized_end=1479
+  _MESSAGEGROUPRESPONSE_MESSAGEPROPERTIESENTRY._serialized_start=1423
+  _MESSAGEGROUPRESPONSE_MESSAGEPROPERTIESENTRY._serialized_end=1479
+  _FILTERNAME._serialized_start=1481
+  _FILTERNAME._serialized_end=1507
+  _FILTER._serialized_start=1509
+  _FILTER._serialized_end=1616
+  _EVENTSEARCHREQUEST._serialized_start=1619
+  _EVENTSEARCHREQUEST._serialized_end=2036
+  _EVENTSEARCHRESPONSE._serialized_start=2038
+  _EVENTSEARCHRESPONSE._serialized_end=2121
+  _MESSAGESEARCHREQUEST._serialized_start=2124
+  _MESSAGESEARCHREQUEST._serialized_end=2610
+  _MESSAGESEARCHRESPONSE._serialized_start=2613
+  _MESSAGESEARCHRESPONSE._serialized_end=2787
+  _MESSAGESTREAMPOINTERS._serialized_start=2789
+  _MESSAGESTREAMPOINTERS._serialized_end=2888
+  _MESSAGESTREAMPOINTER._serialized_start=2890
+  _MESSAGESTREAMPOINTER._serialized_end=3002
+  _MESSAGESTREAM._serialized_start=3004
+  _MESSAGESTREAM._serialized_end=3064
+  _MESSAGESTREAMSRESPONSE._serialized_start=3066
+  _MESSAGESTREAMSRESPONSE._serialized_end=3151
+  _BOOKSREQUEST._serialized_start=3153
+  _BOOKSREQUEST._serialized_end=3167
+  _BOOKSRESPONSE._serialized_start=3169
+  _BOOKSRESPONSE._serialized_end=3232
+  _DATAPROVIDER._serialized_start=3275
+  _DATAPROVIDER._serialized_end=3947
 # @@protoc_insertion_point(module_scope)
```

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/lw_data_provider_pb2.pyi` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/lw_data_provider_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -70,46 +70,38 @@
     START_TIMESTAMP_FIELD_NUMBER: builtins.int
     END_TIMESTAMP_FIELD_NUMBER: builtins.int
     BOOK_ID_FIELD_NUMBER: builtins.int
     MESSAGE_GROUP_FIELD_NUMBER: builtins.int
     SORT_FIELD_NUMBER: builtins.int
     RAW_ONLY_FIELD_NUMBER: builtins.int
     KEEP_OPEN_FIELD_NUMBER: builtins.int
-    RESPONSE_FORMATS_FIELD_NUMBER: builtins.int
     @property
     def start_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     @property
     def end_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     @property
     def book_id(self) -> global___BookId: ...
     @property
     def message_group(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MessageGroupsSearchRequest.Group]: ...
     @property
     def sort(self) -> google.protobuf.wrappers_pb2.BoolValue: ...
     raw_only: builtins.bool
-    """deprecated: use response_formats with only BASE_64 to achieve the same effect"""
-
     keep_open: builtins.bool
-    @property
-    def response_formats(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[typing.Text]:
-        """List of possible response formats (e.g. PARSED or BASE_64)"""
-        pass
     def __init__(self,
         *,
         start_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
         end_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
         book_id: typing.Optional[global___BookId] = ...,
         message_group: typing.Optional[typing.Iterable[global___MessageGroupsSearchRequest.Group]] = ...,
         sort: typing.Optional[google.protobuf.wrappers_pb2.BoolValue] = ...,
         raw_only: builtins.bool = ...,
         keep_open: builtins.bool = ...,
-        response_formats: typing.Optional[typing.Iterable[typing.Text]] = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["book_id",b"book_id","end_timestamp",b"end_timestamp","sort",b"sort","start_timestamp",b"start_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["book_id",b"book_id","end_timestamp",b"end_timestamp","keep_open",b"keep_open","message_group",b"message_group","raw_only",b"raw_only","response_formats",b"response_formats","sort",b"sort","start_timestamp",b"start_timestamp"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["book_id",b"book_id","end_timestamp",b"end_timestamp","keep_open",b"keep_open","message_group",b"message_group","raw_only",b"raw_only","sort",b"sort","start_timestamp",b"start_timestamp"]) -> None: ...
 global___MessageGroupsSearchRequest = MessageGroupsSearchRequest
 
 class MessageStreamsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     BOOK_ID_FIELD_NUMBER: builtins.int
     @property
     def book_id(self) -> global___BookId: ...
@@ -445,15 +437,15 @@
         *,
         message_stream_pointer: typing.Optional[typing.Iterable[global___MessageStreamPointer]] = ...,
         ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["message_stream_pointer",b"message_stream_pointer"]) -> None: ...
 global___MessageStreamPointers = MessageStreamPointers
 
 class MessageStreamPointer(google.protobuf.message.Message):
-    """This object contains the data of the last message in the stream on which
+    """This object contains the data of the last message in the stream on which
     the search has stopped, it is necessary to continue the search from the same point
     """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     MESSAGE_STREAM_FIELD_NUMBER: builtins.int
     LAST_ID_FIELD_NUMBER: builtins.int
     @property
     def message_stream(self) -> global___MessageStream: ...
@@ -513,81 +505,7 @@
     def book_ids(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BookId]: ...
     def __init__(self,
         *,
         book_ids: typing.Optional[typing.Iterable[global___BookId]] = ...,
         ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["book_ids",b"book_ids"]) -> None: ...
 global___BooksResponse = BooksResponse
-
-class PageInfoRequest(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-    BOOK_ID_FIELD_NUMBER: builtins.int
-    START_TIMESTAMP_FIELD_NUMBER: builtins.int
-    END_TIMESTAMP_FIELD_NUMBER: builtins.int
-    RESULT_LIMIT_FIELD_NUMBER: builtins.int
-    @property
-    def book_id(self) -> global___BookId: ...
-    @property
-    def start_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    @property
-    def end_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    @property
-    def result_limit(self) -> google.protobuf.wrappers_pb2.Int32Value: ...
-    def __init__(self,
-        *,
-        book_id: typing.Optional[global___BookId] = ...,
-        start_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
-        end_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
-        result_limit: typing.Optional[google.protobuf.wrappers_pb2.Int32Value] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["book_id",b"book_id","end_timestamp",b"end_timestamp","result_limit",b"result_limit","start_timestamp",b"start_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["book_id",b"book_id","end_timestamp",b"end_timestamp","result_limit",b"result_limit","start_timestamp",b"start_timestamp"]) -> None: ...
-global___PageInfoRequest = PageInfoRequest
-
-class PageInfoResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-    ID_FIELD_NUMBER: builtins.int
-    COMMENT_FIELD_NUMBER: builtins.int
-    STARTED_FIELD_NUMBER: builtins.int
-    ENDED_FIELD_NUMBER: builtins.int
-    UPDATED_FIELD_NUMBER: builtins.int
-    REMOVED_FIELD_NUMBER: builtins.int
-    @property
-    def id(self) -> global___PageId: ...
-    @property
-    def comment(self) -> google.protobuf.wrappers_pb2.StringValue: ...
-    @property
-    def started(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    @property
-    def ended(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    @property
-    def updated(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    @property
-    def removed(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    def __init__(self,
-        *,
-        id: typing.Optional[global___PageId] = ...,
-        comment: typing.Optional[google.protobuf.wrappers_pb2.StringValue] = ...,
-        started: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
-        ended: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
-        updated: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
-        removed: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["comment",b"comment","ended",b"ended","id",b"id","removed",b"removed","started",b"started","updated",b"updated"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["comment",b"comment","ended",b"ended","id",b"id","removed",b"removed","started",b"started","updated",b"updated"]) -> None: ...
-global___PageInfoResponse = PageInfoResponse
-
-class PageId(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-    BOOK_ID_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    @property
-    def book_id(self) -> global___BookId: ...
-    name: typing.Text
-    def __init__(self,
-        *,
-        book_id: typing.Optional[global___BookId] = ...,
-        name: typing.Text = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["book_id",b"book_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["book_id",b"book_id","name",b"name"]) -> None: ...
-global___PageId = PageId
```

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/lw_data_provider_pb2_grpc.py` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/lw_data_provider_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,14 @@
                 response_deserializer=th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.MessageSearchResponse.FromString,
                 )
         self.GetBooks = channel.unary_unary(
                 '/th2.data_provider.lw.DataProvider/GetBooks',
                 request_serializer=th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.BooksRequest.SerializeToString,
                 response_deserializer=th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.BooksResponse.FromString,
                 )
-        self.GetPageInfo = channel.unary_stream(
-                '/th2.data_provider.lw.DataProvider/GetPageInfo',
-                request_serializer=th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.PageInfoRequest.SerializeToString,
-                response_deserializer=th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.PageInfoResponse.FromString,
-                )
 
 
 class DataProviderServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetEvent(self, request, context):
         """returns a single event with the specified id 
@@ -92,34 +87,28 @@
         """creates an event or an event metadata stream that matches the filter. 
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SearchMessageGroups(self, request, context):
-        """
-        Searches for messages groups in specified timestamp
+        """
+        Searches for messages groups in specified timestamp
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetBooks(self, request, context):
-        """Returns the set of books stored in cradle cache
+        """Returns the set of books stored in cradle cache
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetPageInfo(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
 
 def add_DataProviderServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetEvent': grpc.unary_unary_rpc_method_handler(
                     servicer.GetEvent,
                     request_deserializer=th2__grpc__common_dot_common__pb2.EventID.FromString,
                     response_serializer=th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.EventResponse.SerializeToString,
@@ -150,19 +139,14 @@
                     response_serializer=th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.MessageSearchResponse.SerializeToString,
             ),
             'GetBooks': grpc.unary_unary_rpc_method_handler(
                     servicer.GetBooks,
                     request_deserializer=th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.BooksRequest.FromString,
                     response_serializer=th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.BooksResponse.SerializeToString,
             ),
-            'GetPageInfo': grpc.unary_stream_rpc_method_handler(
-                    servicer.GetPageInfo,
-                    request_deserializer=th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.PageInfoRequest.FromString,
-                    response_serializer=th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.PageInfoResponse.SerializeToString,
-            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'th2.data_provider.lw.DataProvider', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -283,24 +267,7 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/th2.data_provider.lw.DataProvider/GetBooks',
             th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.BooksRequest.SerializeToString,
             th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.BooksResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetPageInfo(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/th2.data_provider.lw.DataProvider/GetPageInfo',
-            th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.PageInfoRequest.SerializeToString,
-            th2__grpc__lw__data__provider_dot_lw__data__provider__pb2.PageInfoResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/queue_data_provider.proto` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/queue_data_provider.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/queue_data_provider_pb2.py` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/queue_data_provider_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/queue_data_provider_pb2.pyi` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/queue_data_provider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/queue_data_provider_pb2_grpc.py` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/queue_data_provider_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider/queue_data_provider_service.py` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider/queue_data_provider_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.0.0.dev5795109852/th2_grpc_lw_data_provider.egg-info/SOURCES.txt` & `th2_grpc_lw_data_provider-2.1.0.dev3871883101/th2_grpc_lw_data_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

