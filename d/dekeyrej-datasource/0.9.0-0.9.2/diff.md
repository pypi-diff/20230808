# Comparing `tmp/dekeyrej-datasource-0.9.0.tar.gz` & `tmp/dekeyrej-datasource-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekeyrej-datasource-0.9.0.tar", last modified: Sun Jul 16 19:43:47 2023, max compression
+gzip compressed data, was "dekeyrej-datasource-0.9.2.tar", last modified: Tue Aug  8 01:41:42 2023, max compression
```

## Comparing `dekeyrej-datasource-0.9.0.tar` & `dekeyrej-datasource-0.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 19:43:47.654532 dekeyrej-datasource-0.9.0/
--rw-rw-rw-   0        0        0     1102 2023-07-16 19:30:57.000000 dekeyrej-datasource-0.9.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-07-16 19:09:30.000000 dekeyrej-datasource-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1778 2023-07-16 19:43:47.654532 dekeyrej-datasource-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-07-16 19:08:58.000000 dekeyrej-datasource-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 19:43:47.641205 dekeyrej-datasource-0.9.0/datasourcelib/
--rw-rw-rw-   0        0        0      364 2023-07-16 19:05:58.000000 dekeyrej-datasource-0.9.0/datasourcelib/__init__.py
--rw-rw-rw-   0        0        0     2098 2023-07-03 20:23:02.000000 dekeyrej-datasource-0.9.0/datasourcelib/database.py
--rw-rw-rw-   0        0        0      717 2023-07-03 20:21:30.000000 dekeyrej-datasource-0.9.0/datasourcelib/datasource.py
--rw-rw-rw-   0        0        0     1670 2023-07-03 20:02:55.000000 dekeyrej-datasource-0.9.0/datasourcelib/mongodb.py
--rw-rw-rw-   0        0        0     2611 2023-07-16 19:04:44.000000 dekeyrej-datasource-0.9.0/datasourcelib/postgresdb.py
--rw-rw-rw-   0        0        0     2556 2023-07-16 19:05:35.000000 dekeyrej-datasource-0.9.0/datasourcelib/sqlitedb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 19:43:47.652204 dekeyrej-datasource-0.9.0/dekeyrej_datasource.egg-info/
--rw-rw-rw-   0        0        0     1778 2023-07-16 19:43:47.000000 dekeyrej-datasource-0.9.0/dekeyrej_datasource.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-07-16 19:43:47.000000 dekeyrej-datasource-0.9.0/dekeyrej_datasource.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 19:43:47.000000 dekeyrej-datasource-0.9.0/dekeyrej_datasource.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-16 19:43:47.000000 dekeyrej-datasource-0.9.0/dekeyrej_datasource.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-16 19:43:47.000000 dekeyrej-datasource-0.9.0/dekeyrej_datasource.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      690 2023-07-16 19:43:29.000000 dekeyrej-datasource-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-16 19:43:47.654532 dekeyrej-datasource-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      435 2023-07-16 19:33:18.000000 dekeyrej-datasource-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 19:43:47.653205 dekeyrej-datasource-0.9.0/tests/
--rw-rw-rw-   0        0        0     1721 2023-07-16 19:02:42.000000 dekeyrej-datasource-0.9.0/tests/test_datasource.py
+drwxrwxrwx   0        0        0        0 2023-08-08 01:41:42.038658 dekeyrej-datasource-0.9.2/
+-rw-rw-rw-   0        0        0     1089 2023-08-08 01:02:12.000000 dekeyrej-datasource-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-08-08 01:02:12.000000 dekeyrej-datasource-0.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1892 2023-08-08 01:41:42.037729 dekeyrej-datasource-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-08-08 01:41:16.000000 dekeyrej-datasource-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 01:41:42.026789 dekeyrej-datasource-0.9.2/datasourcelib/
+-rw-rw-rw-   0        0        0      364 2023-08-08 01:02:12.000000 dekeyrej-datasource-0.9.2/datasourcelib/__init__.py
+-rw-rw-rw-   0        0        0     2098 2023-08-08 01:02:12.000000 dekeyrej-datasource-0.9.2/datasourcelib/database.py
+-rw-rw-rw-   0        0        0      717 2023-08-08 01:02:12.000000 dekeyrej-datasource-0.9.2/datasourcelib/datasource.py
+-rw-rw-rw-   0        0        0     1670 2023-08-08 01:02:12.000000 dekeyrej-datasource-0.9.2/datasourcelib/mongodb.py
+-rw-rw-rw-   0        0        0     2611 2023-08-08 01:02:12.000000 dekeyrej-datasource-0.9.2/datasourcelib/postgresdb.py
+-rw-rw-rw-   0        0        0     2556 2023-08-08 01:02:12.000000 dekeyrej-datasource-0.9.2/datasourcelib/sqlitedb.py
+drwxrwxrwx   0        0        0        0 2023-08-08 01:41:42.036728 dekeyrej-datasource-0.9.2/dekeyrej_datasource.egg-info/
+-rw-rw-rw-   0        0        0     1892 2023-08-08 01:41:42.000000 dekeyrej-datasource-0.9.2/dekeyrej_datasource.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-08-08 01:41:42.000000 dekeyrej-datasource-0.9.2/dekeyrej_datasource.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 01:41:42.000000 dekeyrej-datasource-0.9.2/dekeyrej_datasource.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-08-08 01:41:42.000000 dekeyrej-datasource-0.9.2/dekeyrej_datasource.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-08 01:41:42.000000 dekeyrej-datasource-0.9.2/dekeyrej_datasource.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1193 2023-08-08 01:41:16.000000 dekeyrej-datasource-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 01:41:42.038658 dekeyrej-datasource-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      402 2023-08-08 01:41:16.000000 dekeyrej-datasource-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 01:41:42.036728 dekeyrej-datasource-0.9.2/tests/
+-rw-rw-rw-   0        0        0     1721 2023-08-08 01:02:12.000000 dekeyrej-datasource-0.9.2/tests/test_datasource.py
```

### Comparing `dekeyrej-datasource-0.9.0/PKG-INFO` & `dekeyrej-datasource-0.9.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 Metadata-Version: 2.1
 Name: dekeyrej-datasource
-Version: 0.9.0
+Version: 0.9.2
 Summary: Multi-database abstraction layer
+Author: J.DeKeyrel
 Author-email: "J. DeKeyrel" <noneyabusiness@notemail.com>
-License: The MIT License (MIT)
-        Copyright © 2023 <copyright J. DeKeyrel>
+License: MIT License
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        Copyright (c) 2023 J. DeKeyrel
         
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
         
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Example abstraction for multiple database engines
-Also implements a specific schema for storing just the latest record of a record type
+{version='0.9.2'}
+Example abstraction for multiple database engines.
 
-python setup.py pytest
-python setup.py bdist_wheel -d ../wheels
+- example implements a method for storing/retrieving the latest record of rectype 
+    in a hybrid (conventional/json) schema
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dekeyrej-datasource-0.9.0/datasourcelib/database.py` & `dekeyrej-datasource-0.9.2/datasourcelib/database.py`

 * *Files identical despite different names*

### Comparing `dekeyrej-datasource-0.9.0/datasourcelib/datasource.py` & `dekeyrej-datasource-0.9.2/datasourcelib/datasource.py`

 * *Files identical despite different names*

### Comparing `dekeyrej-datasource-0.9.0/datasourcelib/mongodb.py` & `dekeyrej-datasource-0.9.2/datasourcelib/mongodb.py`

 * *Files identical despite different names*

### Comparing `dekeyrej-datasource-0.9.0/datasourcelib/postgresdb.py` & `dekeyrej-datasource-0.9.2/datasourcelib/postgresdb.py`

 * *Files identical despite different names*

### Comparing `dekeyrej-datasource-0.9.0/datasourcelib/sqlitedb.py` & `dekeyrej-datasource-0.9.2/datasourcelib/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `dekeyrej-datasource-0.9.0/dekeyrej_datasource.egg-info/PKG-INFO` & `dekeyrej-datasource-0.9.2/dekeyrej_datasource.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 Metadata-Version: 2.1
 Name: dekeyrej-datasource
-Version: 0.9.0
+Version: 0.9.2
 Summary: Multi-database abstraction layer
+Author: J.DeKeyrel
 Author-email: "J. DeKeyrel" <noneyabusiness@notemail.com>
-License: The MIT License (MIT)
-        Copyright © 2023 <copyright J. DeKeyrel>
+License: MIT License
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        Copyright (c) 2023 J. DeKeyrel
         
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
         
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Example abstraction for multiple database engines
-Also implements a specific schema for storing just the latest record of a record type
+{version='0.9.2'}
+Example abstraction for multiple database engines.
 
-python setup.py pytest
-python setup.py bdist_wheel -d ../wheels
+- example implements a method for storing/retrieving the latest record of rectype 
+    in a hybrid (conventional/json) schema
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dekeyrej-datasource-0.9.0/tests/test_datasource.py` & `dekeyrej-datasource-0.9.2/tests/test_datasource.py`

 * *Files identical despite different names*

