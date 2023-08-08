# Comparing `tmp/fsql-0.5.0.tar.gz` & `tmp/fsql-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/vojta/src/fsql/dist/tmpxjy3sz_k/fsql-0.5.0.tar", last modified: Tue Jun 14 09:40:57 2022, max compression
+gzip compressed data, was "/home/vojta/xrc/fsql/dist/tmpy39yndg1/fsql-0.6.0.tar", last modified: Tue Jun 21 11:45:07 2022, max compression
```

## Comparing `fsql-0.5.0.tar` & `fsql-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vojta     (1000) vojta     (1000)        0 2022-06-14 09:40:57.709585 fsql-0.5.0/
--rw-rw-r--   0 vojta     (1000) vojta     (1000)     1511 2022-05-13 09:26:52.000000 fsql-0.5.0/LICENSE
--rw-rw-r--   0 vojta     (1000) vojta     (1000)     4755 2022-06-14 09:40:57.709585 fsql-0.5.0/PKG-INFO
--rw-rw-r--   0 vojta     (1000) vojta     (1000)     4379 2022-05-13 09:05:38.000000 fsql-0.5.0/README.md
-drwxrwxr-x   0 vojta     (1000) vojta     (1000)        0 2022-06-14 09:40:57.709585 fsql-0.5.0/fsql/
--rw-rw-r--   0 vojta     (1000) vojta     (1000)     2819 2022-05-13 09:10:11.000000 fsql-0.5.0/fsql/__init__.py
--rw-rw-r--   0 vojta     (1000) vojta     (1000)     6931 2022-05-20 11:21:14.000000 fsql-0.5.0/fsql/api.py
--rw-rw-r--   0 vojta     (1000) vojta     (1000)     6068 2022-05-13 09:10:11.000000 fsql-0.5.0/fsql/column_parser.py
--rw-rw-r--   0 vojta     (1000) vojta     (1000)     7478 2022-05-13 09:10:11.000000 fsql-0.5.0/fsql/daterange_utils.py
--rw-rw-r--   0 vojta     (1000) vojta     (1000)     7143 2022-06-14 09:39:49.000000 fsql-0.5.0/fsql/deser.py
--rw-rw-r--   0 vojta     (1000) vojta     (1000)      604 2022-05-13 09:10:11.000000 fsql-0.5.0/fsql/partition.py
--rw-rw-r--   0 vojta     (1000) vojta     (1000)     4184 2022-05-13 09:10:11.000000 fsql-0.5.0/fsql/partition_discovery.py
--rw-rw-r--   0 vojta     (1000) vojta     (1000)     3264 2022-05-13 09:10:11.000000 fsql-0.5.0/fsql/query.py
-drwxrwxr-x   0 vojta     (1000) vojta     (1000)        0 2022-06-14 09:40:57.709585 fsql-0.5.0/fsql.egg-info/
--rw-rw-r--   0 vojta     (1000) vojta     (1000)     4755 2022-06-14 09:40:57.000000 fsql-0.5.0/fsql.egg-info/PKG-INFO
--rw-rw-r--   0 vojta     (1000) vojta     (1000)      355 2022-06-14 09:40:57.000000 fsql-0.5.0/fsql.egg-info/SOURCES.txt
--rw-rw-r--   0 vojta     (1000) vojta     (1000)        1 2022-06-14 09:40:57.000000 fsql-0.5.0/fsql.egg-info/dependency_links.txt
--rw-rw-r--   0 vojta     (1000) vojta     (1000)      121 2022-06-14 09:40:57.000000 fsql-0.5.0/fsql.egg-info/requires.txt
--rw-rw-r--   0 vojta     (1000) vojta     (1000)        5 2022-06-14 09:40:57.000000 fsql-0.5.0/fsql.egg-info/top_level.txt
--rw-rw-r--   0 vojta     (1000) vojta     (1000)      136 2022-05-13 09:05:38.000000 fsql-0.5.0/pyproject.toml
--rw-rw-r--   0 vojta     (1000) vojta     (1000)      652 2022-06-14 09:40:57.709585 fsql-0.5.0/setup.cfg
--rw-rw-r--   0 vojta     (1000) vojta     (1000)      253 2022-05-16 11:16:38.000000 fsql-0.5.0/setup.py
+drwxrwxr-x   0 vojta     (1000) vojta     (1000)        0 2022-06-21 11:45:07.812104 fsql-0.6.0/
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)     1511 2022-06-13 11:59:29.000000 fsql-0.6.0/LICENSE
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)     4755 2022-06-21 11:45:07.812104 fsql-0.6.0/PKG-INFO
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)     4379 2022-06-13 11:59:29.000000 fsql-0.6.0/README.md
+drwxrwxr-x   0 vojta     (1000) vojta     (1000)        0 2022-06-21 11:45:07.812104 fsql-0.6.0/fsql/
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)     2819 2022-06-13 11:59:29.000000 fsql-0.6.0/fsql/__init__.py
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)     7399 2022-06-21 11:41:58.000000 fsql-0.6.0/fsql/api.py
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)     6068 2022-06-13 11:59:29.000000 fsql-0.6.0/fsql/column_parser.py
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)     7478 2022-06-13 11:59:29.000000 fsql-0.6.0/fsql/daterange_utils.py
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)    11711 2022-06-21 11:41:58.000000 fsql-0.6.0/fsql/deser.py
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)      604 2022-06-13 11:59:29.000000 fsql-0.6.0/fsql/partition.py
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)     4184 2022-06-13 11:59:29.000000 fsql-0.6.0/fsql/partition_discovery.py
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)     3264 2022-06-13 11:59:29.000000 fsql-0.6.0/fsql/query.py
+drwxrwxr-x   0 vojta     (1000) vojta     (1000)        0 2022-06-21 11:45:07.812104 fsql-0.6.0/fsql.egg-info/
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)     4755 2022-06-21 11:45:07.000000 fsql-0.6.0/fsql.egg-info/PKG-INFO
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)      355 2022-06-21 11:45:07.000000 fsql-0.6.0/fsql.egg-info/SOURCES.txt
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)        1 2022-06-21 11:45:07.000000 fsql-0.6.0/fsql.egg-info/dependency_links.txt
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)      121 2022-06-21 11:45:07.000000 fsql-0.6.0/fsql.egg-info/requires.txt
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)        5 2022-06-21 11:45:07.000000 fsql-0.6.0/fsql.egg-info/top_level.txt
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)      136 2022-06-13 11:59:29.000000 fsql-0.6.0/pyproject.toml
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)      652 2022-06-21 11:45:07.812104 fsql-0.6.0/setup.cfg
+-rw-rw-r--   0 vojta     (1000) vojta     (1000)      253 2022-06-13 11:59:29.000000 fsql-0.6.0/setup.py
```

### Comparing `fsql-0.5.0/LICENSE` & `fsql-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsql-0.5.0/PKG-INFO` & `fsql-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsql
-Version: 0.5.0
+Version: 0.6.0
 Summary: Metastore-like capabilities for various filesystems
 License: " BSD-3-Clause"
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `fsql-0.5.0/README.md` & `fsql-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fsql-0.5.0/fsql/__init__.py` & `fsql-0.6.0/fsql/__init__.py`

 * *Files identical despite different names*

### Comparing `fsql-0.5.0/fsql/api.py` & `fsql-0.6.0/fsql/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from typing import Optional, Union
 
 import pandas as pd
 from fsspec.spec import AbstractFileSystem
 
 from fsql import get_url_and_fs
 from fsql.column_parser import AUTO_PARSER, ColumnParser
-from fsql.deser import PANDAS_READER, DataReader
+from fsql.deser import PANDAS_READER, DataObject, DataObjectRich, DataReader
 from fsql.partition import Partition
 from fsql.partition_discovery import discover_partitions
 from fsql.query import Query
 
 logger = logging.getLogger(__name__)
 
 
@@ -67,27 +67,32 @@
     return read_partitioned_table(url, query, column_parser, data_reader)
 
 
 def read_partitioned_table(
     url: str,
     query: Query,
     column_parser: ColumnParser = AUTO_PARSER,
-    data_reader: DataReader = PANDAS_READER,
+    data_reader: DataReader[DataObject] = PANDAS_READER,  # type: ignore
     fs: Optional[AbstractFileSystem] = None,
-):
+) -> Union[DataObject, DataObjectRich]:
     """Reads a table rooted at `url`, with partition columns described in `column_parser` and filtered via `query`.
 
     The default values assume `colName1=val/colName2=val` format of the path, and pandas data frame as output format.
     There is no default query -- for reading all partitions, user is supposed to use the always-true query from the
     `query` module.
 
     Note that the provided DataReaders launch a ThreadPoolExecutor when downloading individual files, to speed up I/O.
 
     If `fs` is not provided, a default one is constructed from the url. The instance is then used for all `ls`
     and `open` operations.
+
+    Return type is driven by the `data_reader` -- default behaviour is to return a pandas DataFrame. All provided
+    data readers raise exception whenever any Partition cannot be read, and support `lazy_errors` option which changes
+    the behaviour to collect all exceptions instead and return them together with an object consisting of all that was
+    readable.
     """
     url_suff, fs_default = get_url_and_fs(url)
     fs = fs if fs else fs_default
     # we are relying on the invariant that directory urls end with '/'
     # we thus need to check whether the user is not fooling us
     if not url_suff.endswith("/"):
         if fs.isdir(url_suff):
@@ -104,15 +109,15 @@
 
 def write_object(
     url: str,
     data: Union[pd.DataFrame, io.StringIO, io.BytesIO],
     format: Optional[str] = None,
     format_options: Optional[dict[str, str]] = None,
     fs: Optional[AbstractFileSystem] = None,
-):
+) -> None:
     """Minimalistic function to write an object to a designated location.
 
     * Does not support any table-like semantics -- partition appends or multi-partition inserts,
     * for `io` objects, `seek(0)` and `shutil` write is the behaviour; `format` argument must not be specified,
     * for Data Frames converts to the specified format (only parquet+fastparquet for now), and then it is written
       using the file-like object from fsspec and dataframe's native write.
```

### Comparing `fsql-0.5.0/fsql/column_parser.py` & `fsql-0.6.0/fsql/column_parser.py`

 * *Files identical despite different names*

### Comparing `fsql-0.5.0/fsql/daterange_utils.py` & `fsql-0.6.0/fsql/daterange_utils.py`

 * *Files identical despite different names*

### Comparing `fsql-0.5.0/fsql/partition.py` & `fsql-0.6.0/fsql/partition.py`

 * *Files identical despite different names*

### Comparing `fsql-0.5.0/fsql/partition_discovery.py` & `fsql-0.6.0/fsql/partition_discovery.py`

 * *Files identical despite different names*

### Comparing `fsql-0.5.0/fsql/query.py` & `fsql-0.6.0/fsql/query.py`

 * *Files identical despite different names*

### Comparing `fsql-0.5.0/fsql.egg-info/PKG-INFO` & `fsql-0.6.0/fsql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsql
-Version: 0.5.0
+Version: 0.6.0
 Summary: Metastore-like capabilities for various filesystems
 License: " BSD-3-Clause"
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `fsql-0.5.0/setup.cfg` & `fsql-0.6.0/setup.cfg`

 * *Files identical despite different names*

