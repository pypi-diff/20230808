# Comparing `tmp/tableconv-1.9943.20230729.tar.gz` & `tmp/tableconv-1.9944.20230808.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableconv-1.9943.20230729.tar", last modified: Sat Jul 29 02:02:34 2023, max compression
+gzip compressed data, was "tableconv-1.9944.20230808.tar", last modified: Tue Aug  8 21:45:01 2023, max compression
```

## Comparing `tableconv-1.9943.20230729.tar` & `tableconv-1.9944.20230808.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.199421 tableconv-1.9943.20230729/
--rw-rw-r--   0 john      (1000) john      (1000)     1051 2021-09-03 04:22:14.000000 tableconv-1.9943.20230729/LICENSE
--rw-rw-r--   0 john      (1000) john      (1000)       26 2021-09-03 04:22:14.000000 tableconv-1.9943.20230729/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-07-29 02:02:34.199421 tableconv-1.9943.20230729/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     9258 2023-03-26 03:16:21.000000 tableconv-1.9943.20230729/README.md
--rw-rw-r--   0 john      (1000) john      (1000)       38 2023-07-29 02:02:34.199421 tableconv-1.9943.20230729/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     2232 2023-01-22 04:21:13.000000 tableconv-1.9943.20230729/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.195422 tableconv-1.9943.20230729/tableconv/
--rw-rw-r--   0 john      (1000) john      (1000)      400 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)       73 2023-07-29 02:00:37.000000 tableconv-1.9943.20230729/tableconv/__version__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.195422 tableconv-1.9943.20230729/tableconv/adapters/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2021-09-03 04:22:14.000000 tableconv-1.9943.20230729/tableconv/adapters/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.199421 tableconv-1.9943.20230729/tableconv/adapters/df/
--rw-rw-r--   0 john      (1000) john      (1000)      926 2023-01-27 19:23:04.000000 tableconv-1.9943.20230729/tableconv/adapters/df/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4264 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/ascii.py
--rw-rw-r--   0 john      (1000) john      (1000)    14948 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/aws_athena.py
--rw-rw-r--   0 john      (1000) john      (1000)     1081 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/aws_dynamodb.py
--rw-r--r--   0 john      (1000) john      (1000)     2394 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/aws_logs.py
--rw-rw-r--   0 john      (1000) john      (1000)     1696 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/base.py
--rw-rw-r--   0 john      (1000) john      (1000)      403 2022-01-02 03:01:01.000000 tableconv-1.9943.20230729/tableconv/adapters/df/example.py
--rw-rw-r--   0 john      (1000) john      (1000)     2526 2023-05-30 16:53:38.000000 tableconv-1.9943.20230729/tableconv/adapters/df/file_adapter_mixin.py
--rw-rw-r--   0 john      (1000) john      (1000)    13123 2023-07-29 01:59:21.000000 tableconv-1.9943.20230729/tableconv/adapters/df/gsheets.py
--rw-rw-r--   0 john      (1000) john      (1000)      339 2023-06-26 23:24:34.000000 tableconv-1.9943.20230729/tableconv/adapters/df/jira.py
--rw-rw-r--   0 john      (1000) john      (1000)     6463 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/json.py
--rw-rw-r--   0 john      (1000) john      (1000)     1876 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/nested_list.py
--rw-r--r--   0 john      (1000) john      (1000)     1509 2023-03-26 03:15:45.000000 tableconv-1.9943.20230729/tableconv/adapters/df/numbers.py
--rw-rw-r--   0 john      (1000) john      (1000)     8885 2023-06-30 22:42:07.000000 tableconv-1.9943.20230729/tableconv/adapters/df/pandas_io.py
--rw-rw-r--   0 john      (1000) john      (1000)     1642 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/python.py
--rw-rw-r--   0 john      (1000) john      (1000)     5805 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/rdbms.py
--rw-rw-r--   0 john      (1000) john      (1000)     2494 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/smart_sheet.py
--rw-r--r--   0 john      (1000) john      (1000)      866 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/sql_literal.py
--rw-rw-r--   0 john      (1000) john      (1000)     7489 2023-06-16 22:05:58.000000 tableconv-1.9943.20230729/tableconv/adapters/df/sumo_logic.py
--rw-rw-r--   0 john      (1000) john      (1000)     2999 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/text_array.py
--rw-rw-r--   0 john      (1000) john      (1000)     1644 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/adapters/df/yaml.py
--rw-rw-r--   0 john      (1000) john      (1000)    15649 2023-06-16 22:00:59.000000 tableconv-1.9943.20230729/tableconv/core.py
--rw-r--r--   0 john      (1000) john      (1000)     2301 2023-07-29 01:57:22.000000 tableconv-1.9943.20230729/tableconv/exceptions.py
--rw-rw-r--   0 john      (1000) john      (1000)     3096 2023-06-30 23:18:47.000000 tableconv-1.9943.20230729/tableconv/in_memory_query.py
--rw-rw-r--   0 john      (1000) john      (1000)     5836 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/interactive.py
--rw-rw-r--   0 john      (1000) john      (1000)    11215 2023-06-30 23:07:40.000000 tableconv-1.9943.20230729/tableconv/main.py
--rw-rw-r--   0 john      (1000) john      (1000)      726 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/parse_time.py
--rw-rw-r--   0 john      (1000) john      (1000)     1469 2023-01-22 04:03:54.000000 tableconv-1.9943.20230729/tableconv/uri.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.195422 tableconv-1.9943.20230729/tableconv.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     1242 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       66 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      243 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       27 2023-07-29 02:02:34.000000 tableconv-1.9943.20230729/tableconv.egg-info/top_level.txt
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-29 02:02:34.199421 tableconv-1.9943.20230729/tableconv_daemon/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-01-15 04:13:45.000000 tableconv-1.9943.20230729/tableconv_daemon/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     9537 2023-03-26 02:56:00.000000 tableconv-1.9943.20230729/tableconv_daemon/main.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-08 21:45:01.800892 tableconv-1.9944.20230808/
+-rw-rw-r--   0 john      (1000) john      (1000)     1051 2021-09-03 04:22:14.000000 tableconv-1.9944.20230808/LICENSE
+-rw-rw-r--   0 john      (1000) john      (1000)       26 2021-09-03 04:22:14.000000 tableconv-1.9944.20230808/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-08-08 21:45:01.796892 tableconv-1.9944.20230808/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     9258 2023-03-26 03:16:21.000000 tableconv-1.9944.20230808/README.md
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2023-08-08 21:45:01.800892 tableconv-1.9944.20230808/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     2232 2023-01-22 04:21:13.000000 tableconv-1.9944.20230808/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-08 21:45:01.796892 tableconv-1.9944.20230808/tableconv/
+-rw-rw-r--   0 john      (1000) john      (1000)      400 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)       73 2023-08-08 21:44:17.000000 tableconv-1.9944.20230808/tableconv/__version__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-08 21:45:01.796892 tableconv-1.9944.20230808/tableconv/adapters/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2021-09-03 04:22:14.000000 tableconv-1.9944.20230808/tableconv/adapters/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-08 21:45:01.796892 tableconv-1.9944.20230808/tableconv/adapters/df/
+-rw-rw-r--   0 john      (1000) john      (1000)      926 2023-01-27 19:23:04.000000 tableconv-1.9944.20230808/tableconv/adapters/df/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4264 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/ascii.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14948 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/aws_athena.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1081 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/aws_dynamodb.py
+-rw-r--r--   0 john      (1000) john      (1000)     2394 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/aws_logs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1696 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)      403 2022-01-02 03:01:01.000000 tableconv-1.9944.20230808/tableconv/adapters/df/example.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2526 2023-05-30 16:53:38.000000 tableconv-1.9944.20230808/tableconv/adapters/df/file_adapter_mixin.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13316 2023-08-07 22:28:07.000000 tableconv-1.9944.20230808/tableconv/adapters/df/gsheets.py
+-rw-rw-r--   0 john      (1000) john      (1000)      339 2023-06-26 23:24:34.000000 tableconv-1.9944.20230808/tableconv/adapters/df/jira.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6463 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/json.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1876 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/nested_list.py
+-rw-r--r--   0 john      (1000) john      (1000)     1509 2023-03-26 03:15:45.000000 tableconv-1.9944.20230808/tableconv/adapters/df/numbers.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8885 2023-06-30 22:42:07.000000 tableconv-1.9944.20230808/tableconv/adapters/df/pandas_io.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1642 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/python.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5805 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/rdbms.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2494 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/smart_sheet.py
+-rw-r--r--   0 john      (1000) john      (1000)      866 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/sql_literal.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7489 2023-06-16 22:05:58.000000 tableconv-1.9944.20230808/tableconv/adapters/df/sumo_logic.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2999 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/text_array.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1644 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/adapters/df/yaml.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15651 2023-08-08 00:15:59.000000 tableconv-1.9944.20230808/tableconv/core.py
+-rw-r--r--   0 john      (1000) john      (1000)     2301 2023-07-29 01:57:22.000000 tableconv-1.9944.20230808/tableconv/exceptions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3096 2023-06-30 23:18:47.000000 tableconv-1.9944.20230808/tableconv/in_memory_query.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5836 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/interactive.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11215 2023-06-30 23:07:40.000000 tableconv-1.9944.20230808/tableconv/main.py
+-rw-rw-r--   0 john      (1000) john      (1000)      726 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/parse_time.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1469 2023-01-22 04:03:54.000000 tableconv-1.9944.20230808/tableconv/uri.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-08 21:45:01.796892 tableconv-1.9944.20230808/tableconv.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-08-08 21:45:01.000000 tableconv-1.9944.20230808/tableconv.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     1242 2023-08-08 21:45:01.000000 tableconv-1.9944.20230808/tableconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-08-08 21:45:01.000000 tableconv-1.9944.20230808/tableconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       66 2023-08-08 21:45:01.000000 tableconv-1.9944.20230808/tableconv.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      243 2023-08-08 21:45:01.000000 tableconv-1.9944.20230808/tableconv.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       27 2023-08-08 21:45:01.000000 tableconv-1.9944.20230808/tableconv.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-08-08 21:45:01.796892 tableconv-1.9944.20230808/tableconv_daemon/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-01-15 04:13:45.000000 tableconv-1.9944.20230808/tableconv_daemon/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9537 2023-03-26 02:56:00.000000 tableconv-1.9944.20230808/tableconv_daemon/main.py
```

### Comparing `tableconv-1.9943.20230729/LICENSE` & `tableconv-1.9944.20230808/LICENSE`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/PKG-INFO` & `tableconv-1.9944.20230808/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableconv
-Version: 1.9943.20230729
+Version: 1.9944.20230808
 Summary: CLI data plumbing tool
 Home-page: https://github.com/personalcomputer/tableconv
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tableconv-1.9943.20230729/README.md` & `tableconv-1.9944.20230808/README.md`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/setup.py` & `tableconv-1.9944.20230808/setup.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/__init__.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/__init__.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/ascii.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/ascii.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/aws_athena.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/aws_athena.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/aws_dynamodb.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/aws_dynamodb.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/aws_logs.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/aws_logs.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/base.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/base.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/file_adapter_mixin.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/file_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/gsheets.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/gsheets.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,19 +162,19 @@
             googlesheets.spreadsheets()
             .batchUpdate(spreadsheetId=spreadsheet_id, body={"requests": [request]})
             .execute()
         )
         return response["replies"][0]["addSheet"]["properties"]["sheetId"]
 
     @staticmethod
-    def _extend_sheet(googlesheets, spreadsheet_id, sheet_id, new_total_rows):
+    def _reshape_sheet(googlesheets, spreadsheet_id, sheet_id, columns, rows):
         request = {
             "updateSheetProperties": {
                 "properties": {
-                    "gridProperties": {"rowCount": new_total_rows},
+                    "gridProperties": {"columnCount": columns, "rowCount": rows},
                     "sheetId": sheet_id,
                 },
                 "fields": "gridProperties.rowCount",
             }
         }
         googlesheets.spreadsheets().batchUpdate(spreadsheetId=spreadsheet_id, body={"requests": [request]}).execute()
 
@@ -229,18 +229,19 @@
         serialized_header = [list(df.columns)]
         googlesheets = GoogleSheetsAdapter._get_googleapiclient_client("sheets", "v4")
 
         # Create new spreadsheet, if specified.
         columns = len(df.columns)
         rows = len(df.values)
         new_sheet = None
+        reformat = True
         start_row = 1
         if parsed_uri.authority.lower().strip() == ":new:":
             if if_exists != "fail":
-                raise InvalidParamsError("only if_exists=fail supported for new spreadsheets")
+                raise InvalidParamsError("only if_exists=fail supported for :new: spreadsheets")
             datetime_formatted = datetime.datetime.now(tz=datetime.timezone.utc).strftime("%Y-%m-%d %H:%M:%S UTC")
             spreadsheet_name = params.get("name", f"Untitled {datetime_formatted}")
             spreadsheet_id = GoogleSheetsAdapter._create_spreadsheet(
                 googlesheets, spreadsheet_name, sheet_name, columns, rows
             )
             sheet_id = 0
 
@@ -260,44 +261,46 @@
             except googleapiclient.errors.HttpError as exc:
                 if f'A sheet with the name "{sheet_name}" already exists' not in str(exc):
                     raise
                 if if_exists == "fail":
                     raise TableAlreadyExistsError(exc.reason) from exc
                 new_sheet = False
             if not new_sheet:
+                spreadsheet_data = googlesheets.spreadsheets().get(spreadsheetId=spreadsheet_id).execute()
+                sheet = get_sheet_properties(spreadsheet_data, sheet_name=sheet_name)
+                sheet_id = sheet["sheetId"]
                 if if_exists == "replace":
+                    GoogleSheetsAdapter._reshape_sheet(googlesheets, spreadsheet_id, sheet_id, columns=columns, rows=rows)
                     # delete it..
-                    raise NotImplementedError("Sheet if_exists=replace not implemented yet")
+                    # raise NotImplementedError("Sheet if_exists=replace not implemented yet")
                 elif if_exists == "append":
-                    spreadsheet_data = googlesheets.spreadsheets().get(spreadsheetId=spreadsheet_id).execute()
-                    sheet = get_sheet_properties(spreadsheet_data, sheet_name=sheet_name)
+                    reformat = False
                     existing_rows = sheet["gridProperties"]["rowCount"]
                     existing_columns = sheet["gridProperties"]["columnCount"]
                     if existing_columns != columns:
                         raise AppendSchemeConflictError(f"Cannot append to {sheet_name} - columns don't match")
-                    sheet_id = sheet["sheetId"]
-                    total_rows = existing_rows + columns
-                    GoogleSheetsAdapter._extend_sheet(googlesheets, spreadsheet_id, sheet_id, new_total_rows=total_rows)
+                    total_rows = existing_rows + rows
+                    GoogleSheetsAdapter._reshape_sheet(googlesheets, spreadsheet_id, sheet_id, columns=columns, rows=total_rows)
                     start_row = existing_rows + 1
                 else:
                     raise AssertionError
 
         # Insert data
         serialized_cells = serialized_records
-        if new_sheet:
+        if reformat:
             serialized_cells = serialized_header + serialized_records
         googlesheets.spreadsheets().values().update(
             spreadsheetId=spreadsheet_id,
             range=f"{sheet_name}!A{start_row}",
             valueInputOption="RAW",
             body={"values": serialized_cells},
         ).execute()
 
         # Format
-        if new_sheet:
+        if reformat:
             googlesheets.spreadsheets().batchUpdate(
                 spreadsheetId=spreadsheet_id,
                 body={
                     "requests": [
                         {
                             "updateSheetProperties": {
                                 "properties": {"sheetId": sheet_id, "gridProperties": {"frozenRowCount": 1}},
```

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/json.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/json.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/nested_list.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/nested_list.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/numbers.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/numbers.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/pandas_io.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/pandas_io.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/python.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/python.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/rdbms.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/rdbms.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/smart_sheet.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/smart_sheet.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/sql_literal.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/sql_literal.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/sumo_logic.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/sumo_logic.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/text_array.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/text_array.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/adapters/df/yaml.py` & `tableconv-1.9944.20230808/tableconv/adapters/df/yaml.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/core.py` & `tableconv-1.9944.20230808/tableconv/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             table and there is a schema mismatch)
         """
         scheme = parse_uri(url).scheme
         try:
             write_adapter = write_adapters[scheme]
         except KeyError:
             raise UnrecognizedFormatError(
-                f'Unsupported scheme {scheme}. Supported schemes: {", ".join(write_adapters.keys())}'
+                f'Unsupported scheme "{scheme}". Supported schemes: {", ".join(write_adapters.keys())}'
             )
 
         if params:
             # TODO: This is a total hack! Implementing real structured table references, including structured passing of
             # params to adapters, is still pending. Right now everything is stringly-typed internally.
             assert "?" not in url
             url += f"?{urllib.parse.urlencode(params)}"
```

### Comparing `tableconv-1.9943.20230729/tableconv/exceptions.py` & `tableconv-1.9944.20230808/tableconv/exceptions.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/in_memory_query.py` & `tableconv-1.9944.20230808/tableconv/in_memory_query.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/interactive.py` & `tableconv-1.9944.20230808/tableconv/interactive.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/main.py` & `tableconv-1.9944.20230808/tableconv/main.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/parse_time.py` & `tableconv-1.9944.20230808/tableconv/parse_time.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv/uri.py` & `tableconv-1.9944.20230808/tableconv/uri.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv.egg-info/PKG-INFO` & `tableconv-1.9944.20230808/tableconv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableconv
-Version: 1.9943.20230729
+Version: 1.9944.20230808
 Summary: CLI data plumbing tool
 Home-page: https://github.com/personalcomputer/tableconv
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tableconv-1.9943.20230729/tableconv.egg-info/SOURCES.txt` & `tableconv-1.9944.20230808/tableconv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tableconv-1.9943.20230729/tableconv_daemon/main.py` & `tableconv-1.9944.20230808/tableconv_daemon/main.py`

 * *Files identical despite different names*

