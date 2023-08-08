# Comparing `tmp/layout2svg-0.1.0.tar.gz` & `tmp/layout2svg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layout2svg-0.1.0.tar", max compression
+gzip compressed data, was "layout2svg-0.1.1.tar", max compression
```

## Comparing `layout2svg-0.1.0.tar` & `layout2svg-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       22 2023-08-08 02:48:25.552267 layout2svg-0.1.0/layout2svg/__init__.py
--rw-r--r--   0        0        0     2221 2023-08-08 04:08:56.505191 layout2svg-0.1.0/layout2svg/data.py
--rw-r--r--   0        0        0     7593 2023-08-08 04:08:56.529512 layout2svg-0.1.0/layout2svg/layout2svg.py
--rw-r--r--   0        0        0      797 2023-08-08 04:27:56.977938 layout2svg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      847 2023-08-08 04:30:19.677949 layout2svg-0.1.0/setup.py
--rw-r--r--   0        0        0      567 2023-08-08 04:30:19.678179 layout2svg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-08-08 02:48:25.552267 layout2svg-0.1.1/layout2svg/__init__.py
+-rw-r--r--   0        0        0     2221 2023-08-08 04:08:56.505191 layout2svg-0.1.1/layout2svg/data.py
+-rw-r--r--   0        0        0     7593 2023-08-08 04:08:56.529512 layout2svg-0.1.1/layout2svg/layout2svg.py
+-rw-r--r--   0        0        0      797 2023-08-08 04:33:15.107423 layout2svg-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      847 2023-08-08 04:33:17.607514 layout2svg-0.1.1/setup.py
+-rw-r--r--   0        0        0      567 2023-08-08 04:33:17.607727 layout2svg-0.1.1/PKG-INFO
```

### Comparing `layout2svg-0.1.0/layout2svg/data.py` & `layout2svg-0.1.1/layout2svg/data.py`

 * *Files identical despite different names*

### Comparing `layout2svg-0.1.0/layout2svg/layout2svg.py` & `layout2svg-0.1.1/layout2svg/layout2svg.py`

 * *Files identical despite different names*

### Comparing `layout2svg-0.1.0/pyproject.toml` & `layout2svg-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "layout2svg"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["dasdias <das.dias6@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docopt = "^0.6.2"
 klayout = "^0.28.10"
```

### Comparing `layout2svg-0.1.0/setup.py` & `layout2svg-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'lxml>=4.9.3,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['layout2svg = bin.layout2svg:main']}
 
 setup_kwargs = {
     'name': 'layout2svg',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': None,
     'author': 'dasdias',
     'author_email': 'das.dias6@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `layout2svg-0.1.0/PKG-INFO` & `layout2svg-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layout2svg
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: dasdias
 Author-email: das.dias6@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

