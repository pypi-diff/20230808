# Comparing `tmp/toRST-0.1.0.tar.gz` & `tmp/toRST-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toRST-0.1.0.tar", last modified: Sat Jul 22 16:41:35 2023, max compression
+gzip compressed data, was "toRST-0.1.1.tar", last modified: Tue Aug  8 00:30:40 2023, max compression
```

## Comparing `toRST-0.1.0.tar` & `toRST-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 16:41:35.033493 toRST-0.1.0/
--rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.1.0/LICENSE
--rw-r--r--   0 jreyno     (501) staff       (20)     2787 2023-07-22 16:41:35.033565 toRST-0.1.0/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)     1369 2023-07-22 16:36:50.000000 toRST-0.1.0/README.md
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 16:41:35.031050 toRST-0.1.0/csv2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.1.0/csv2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      836 2023-07-21 03:11:50.000000 toRST-0.1.0/csv2rst/csv2rst.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 16:41:35.031632 toRST-0.1.0/funcs/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.1.0/funcs/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.1.0/funcs/command.py
--rw-r--r--   0 jreyno     (501) staff       (20)      994 2023-07-22 16:39:19.000000 toRST-0.1.0/funcs/funcs.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 16:41:35.031935 toRST-0.1.0/json2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.1.0/json2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.1.0/json2rst/json2rst.py
--rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.1.0/pyproject.toml
--rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-22 16:41:35.033819 toRST-0.1.0/setup.cfg
--rw-r--r--   0 jreyno     (501) staff       (20)     1706 2023-07-22 16:37:44.000000 toRST-0.1.0/setup.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 16:41:35.032114 toRST-0.1.0/tests/
--rw-r--r--   0 jreyno     (501) staff       (20)     1471 2023-07-22 16:40:01.000000 toRST-0.1.0/tests/test_toRST_toRST.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 16:41:35.032626 toRST-0.1.0/toRST/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.1.0/toRST/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     2654 2023-07-22 02:23:35.000000 toRST-0.1.0/toRST/toRST.py
--rw-r--r--   0 jreyno     (501) staff       (20)      332 2023-07-21 01:49:45.000000 toRST-0.1.0/toRST/write.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 16:41:35.033399 toRST-0.1.0/toRST.egg-info/
--rw-r--r--   0 jreyno     (501) staff       (20)     2787 2023-07-22 16:41:35.000000 toRST-0.1.0/toRST.egg-info/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-22 16:41:35.000000 toRST-0.1.0/toRST.egg-info/SOURCES.txt
--rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-22 16:41:35.000000 toRST-0.1.0/toRST.egg-info/dependency_links.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-22 16:41:35.000000 toRST-0.1.0/toRST.egg-info/entry_points.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-22 16:41:35.000000 toRST-0.1.0/toRST.egg-info/top_level.txt
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-08-08 00:30:40.366306 toRST-0.1.1/
+-rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.1.1/LICENSE
+-rw-r--r--   0 jreyno     (501) staff       (20)     2806 2023-08-08 00:30:40.366365 toRST-0.1.1/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)     1388 2023-08-08 00:27:41.000000 toRST-0.1.1/README.md
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-08-08 00:30:40.363973 toRST-0.1.1/csv2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.1.1/csv2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      836 2023-07-21 03:11:50.000000 toRST-0.1.1/csv2rst/csv2rst.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-08-08 00:30:40.364537 toRST-0.1.1/funcs/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.1.1/funcs/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.1.1/funcs/command.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     1204 2023-08-08 00:24:50.000000 toRST-0.1.1/funcs/funcs.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-08-08 00:30:40.364880 toRST-0.1.1/json2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.1.1/json2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      896 2023-08-08 00:24:50.000000 toRST-0.1.1/json2rst/json2rst.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.1.1/pyproject.toml
+-rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-08-08 00:30:40.366608 toRST-0.1.1/setup.cfg
+-rw-r--r--   0 jreyno     (501) staff       (20)     1725 2023-08-08 00:28:14.000000 toRST-0.1.1/setup.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-08-08 00:30:40.365080 toRST-0.1.1/tests/
+-rw-r--r--   0 jreyno     (501) staff       (20)     1901 2023-08-08 00:24:50.000000 toRST-0.1.1/tests/test_toRST_toRST.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-08-08 00:30:40.365518 toRST-0.1.1/toRST/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.1.1/toRST/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     2654 2023-07-30 13:47:34.000000 toRST-0.1.1/toRST/toRST.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      332 2023-07-21 01:49:45.000000 toRST-0.1.1/toRST/write.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-08-08 00:30:40.366183 toRST-0.1.1/toRST.egg-info/
+-rw-r--r--   0 jreyno     (501) staff       (20)     2806 2023-08-08 00:30:40.000000 toRST-0.1.1/toRST.egg-info/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-08-08 00:30:40.000000 toRST-0.1.1/toRST.egg-info/SOURCES.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-08-08 00:30:40.000000 toRST-0.1.1/toRST.egg-info/dependency_links.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-08-08 00:30:40.000000 toRST-0.1.1/toRST.egg-info/entry_points.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-08-08 00:30:40.000000 toRST-0.1.1/toRST.egg-info/top_level.txt
```

### Comparing `toRST-0.1.0/LICENSE` & `toRST-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toRST-0.1.0/PKG-INFO` & `toRST-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
         
@@ -44,15 +44,15 @@
 <br>
 
 **CLI Usage**
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
-torst file1.csv file2.json -o ./outputfolder
+torst file1.csv file2.json -o /outputfolder
 ```
 
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are 
@@ -73,8 +73,8 @@
 ```python
 from toRST.toRST import Table
 ```
 Convert file1.csv into RST string
 ```python
 rst_table = Table('file1.csv').build_table()
 ```
-Can also convert ```list[list or tuple or dict]``` into RST by passing the object into the ```Table``` class<br>
+Can also convert ```list[list or tuple or dict] and dict[str, list]``` into RST by passing the object into the ```Table``` class<br>
```

### Comparing `toRST-0.1.0/README.md` & `toRST-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 <br>
 
 **CLI Usage**
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
-torst file1.csv file2.json -o ./outputfolder
+torst file1.csv file2.json -o /outputfolder
 ```
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are 
   supported, but additional formats will be added.
@@ -51,13 +51,13 @@
 ```python
 from toRST.toRST import Table
 ```
 Convert file1.csv into RST string
 ```python
 rst_table = Table('file1.csv').build_table()
 ```
-Can also convert ```list[list or tuple or dict]``` into RST by passing the object into the ```Table``` class<br> 
+Can also convert ```list[list or tuple or dict] and dict[str, list]``` into RST by passing the object into the ```Table``` class<br> 
 
 **What toRST was built for**
 ----------------------------
 
 While building [mlb-positive-ev](https://github.com/jrey999/mlb-positive-ev), I wanted a quick and readable output of a SQLite query and couldn't find anything suitable.
```

### Comparing `toRST-0.1.0/csv2rst/csv2rst.py` & `toRST-0.1.1/csv2rst/csv2rst.py`

 * *Files identical despite different names*

### Comparing `toRST-0.1.0/funcs/command.py` & `toRST-0.1.1/funcs/command.py`

 * *Files identical despite different names*

### Comparing `toRST-0.1.0/funcs/funcs.py` & `toRST-0.1.1/funcs/funcs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from csv2rst.csv2rst import from_csv
-from json2rst.json2rst import from_json
+from json2rst.json2rst import from_json, from_list_values
 
 
 def get_extension(file: str) -> str:
 
     return file.split(".")[-1].lower()
 
 def handle_file(file: str) -> list[list]:
@@ -14,17 +14,19 @@
     elif extension == "json":
         return from_json(file)
     else:
         raise ValueError(f"{extension} files not currently supported")
 
 def handle_raw(input: list[list or dict]) -> list[list]:
 
-    if not isinstance(input, list):
-        raise ValueError("input must be of type list[list or dict or tuple]")
+    if not isinstance(input, list) or isinstance(input, dict):
+        raise ValueError("input must be of type list[list or dict or tuple] or dict[str, list]")
     else:
         if isinstance(input[0], list):
             return input
         elif isinstance(input[0], dict):
             return [[key for key in input[0].keys()]] + [list(row.values()) for row in input[1:]]
         elif isinstance(input[0], tuple):
             return [list(row) for row in input]
-        else: raise ValueError("input must be of type list[list or dict or tuple]")
+        elif isinstance(input, dict) and isinstance(list(input.values())[0], list):
+            return from_list_values(input)
+        else: raise ValueError("input must be of type list[list or dict or tuple] or dict[str, list]")
```

### Comparing `toRST-0.1.0/setup.cfg` & `toRST-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torst
-version = 0.1.0
+version = 0.1.1
 author = John Reynolds
 author_email = reynoldsjohngreg@gmail.com
 description = Convert various data formats to reStructuredText tables.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jrey999/toRST
 project_urls =
```

### Comparing `toRST-0.1.0/setup.py` & `toRST-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 <br>
 
 **CLI Usage**
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
-torst file1.csv file2.json -o ./outputfolder
+torst file1.csv file2.json -o /outputfolder
 ```
 
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are 
@@ -55,22 +55,22 @@
 ```python
 from toRST.toRST import Table
 ```
 Convert file1.csv into RST string
 ```python
 rst_table = Table('file1.csv').build_table()
 ```
-Can also convert ```list[list or tuple or dict]``` into RST by passing the object into the ```Table``` class<br> 
+Can also convert ```list[list or tuple or dict] and dict[str, list]``` into RST by passing the object into the ```Table``` class<br> 
 """.strip()
 
 with open('LICENSE') as f:
     license = f.read()
 setup(
     name='toRST',
-    version='0.1.0',
+    version='0.1.1',
     description='Command line tool for converting CSV and JSON files into reStructuredText Tables.',
     long_description=readme,
     author='John Reynolds',
     author_email='reynoldsjohngreg@gmail.com',
     url='https://github.com/jrey999/toRST',
     license=license,
     packages=find_packages(exclude=('tests',)),
```

### Comparing `toRST-0.1.0/tests/test_toRST_toRST.py` & `toRST-0.1.1/tests/test_toRST_toRST.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from toRST.toRST import Table
 from csv2rst.csv2rst import clean_csv
+from json2rst.json2rst import from_list_values
 from funcs.funcs import handle_raw
-import pytest
+import pytest, json
 
 
 @pytest.fixture
 def empty_table():
 
-    yield Table('tests/csv/empty.csv')
+    yield Table('tests/data/empty.csv')
 
 @pytest.fixture
 def large_table():
 
-    yield Table('tests/csv/large.csv')
+    yield Table('tests/data/large.csv')
 
 @pytest.fixture
 def small_table():
 
-    yield Table('tests/csv/small.csv')
+    yield Table('tests/data/small.csv')
 
 def test_headers(empty_table, large_table, small_table) -> None:
 
     assert empty_table.headers == ["No","Data","Here"]
     assert large_table.headers == ["First Name","Last Name","Job Title","Biography"]
     assert small_table.headers == ["Header1","Header2","Header3"]
 
@@ -35,12 +36,22 @@
 
     assert clean_csv([["ab", "cd", "ef", "gh", "", ""], ["ba", "dc", "fe", "hg", "", ""]]) == [["ab", "cd", "ef", "gh"], ["ba", "dc", "fe", "hg"]]
 
 def test_handle_raw() -> None:
 
     with pytest.raises(ValueError) as value_error:
         handle_raw({"key1": "value1", "key2": "value2"})
-    assert str(value_error.value) == "input must be of type list[list or dict or tuple]"
+    assert str(value_error.value) == "input must be of type list[list or dict or tuple] or dict[str, list]"
 
     with pytest.raises(ValueError) as value_error:
         handle_raw(["value", "value", "value", "value"])
-    assert str(value_error.value) == "input must be of type list[list or dict or tuple]"
+    assert str(value_error.value) == "input must be of type list[list or dict or tuple] or dict[str, list]"
+
+def test_from_list_values() -> None:
+    data = json.load(open("tests/data/list_values.json"))
+    assert from_list_values(data) == [
+        ['height', 'weight', 'age', 'country'],
+        [170.5, 70.4, 28, 'USA'],
+        [180.3, 90.2, 32, 'Canada'],
+        [176.8, 80.5, 31, 'UK'],
+        [182.6, 75.3, 36, 'Australia']
+        ]
```

### Comparing `toRST-0.1.0/toRST/toRST.py` & `toRST-0.1.1/toRST/toRST.py`

 * *Files identical despite different names*

### Comparing `toRST-0.1.0/toRST.egg-info/PKG-INFO` & `toRST-0.1.1/toRST.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
         
@@ -44,15 +44,15 @@
 <br>
 
 **CLI Usage**
 -------------
 example<br>
   Convert file1.csv and file2.json into RST
 ```bash
-torst file1.csv file2.json -o ./outputfolder
+torst file1.csv file2.json -o /outputfolder
 ```
 
 **Positional Arguments**:
 ------------------------
 
 inputs
   One or more input files to convert to RST. Currently only CSV and JSON files are 
@@ -73,8 +73,8 @@
 ```python
 from toRST.toRST import Table
 ```
 Convert file1.csv into RST string
 ```python
 rst_table = Table('file1.csv').build_table()
 ```
-Can also convert ```list[list or tuple or dict]``` into RST by passing the object into the ```Table``` class<br>
+Can also convert ```list[list or tuple or dict] and dict[str, list]``` into RST by passing the object into the ```Table``` class<br>
```

