# Comparing `tmp/dubo-0.2.4.tar.gz` & `tmp/dubo-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dubo-0.2.4.tar", max compression
+gzip compressed data, was "dubo-0.2.5.tar", max compression
```

## Comparing `dubo-0.2.4.tar` & `dubo-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1092 2023-01-05 00:01:04.309003 dubo-0.2.4/LICENSE
--rw-r--r--   0        0        0      171 2023-01-05 05:56:58.393399 dubo-0.2.4/README.md
--rw-r--r--   0        0        0      194 2023-01-05 10:20:42.201716 dubo-0.2.4/dubo/__init__.py
--rw-r--r--   0        0        0      119 2023-07-05 20:05:03.562011 dubo-0.2.4/dubo/__version__.py
--rw-r--r--   0        0        0     3311 2023-07-05 20:08:11.607878 dubo-0.2.4/dubo/ask_dubo.py
--rw-r--r--   0        0        0      336 2023-07-05 20:04:00.514700 dubo-0.2.4/dubo/config.py
--rw-r--r--   0        0        0      556 2023-07-05 20:18:48.836736 dubo-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 dubo-0.2.4/setup.py
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 dubo-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-01-05 00:01:04.309003 dubo-0.2.5/LICENSE
+-rw-r--r--   0        0        0      171 2023-01-05 05:56:58.393399 dubo-0.2.5/README.md
+-rw-r--r--   0        0        0      208 2023-08-07 20:42:44.194834 dubo-0.2.5/dubo/__init__.py
+-rw-r--r--   0        0        0      119 2023-08-07 20:37:29.082311 dubo-0.2.5/dubo/__version__.py
+-rw-r--r--   0        0        0     5509 2023-08-07 20:42:23.669475 dubo-0.2.5/dubo/ask_dubo.py
+-rw-r--r--   0        0        0      474 2023-08-07 20:43:24.628194 dubo-0.2.5/dubo/config.py
+-rw-r--r--   0        0        0      592 2023-08-07 20:37:29.084509 dubo-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 dubo-0.2.5/setup.py
+-rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 dubo-0.2.5/PKG-INFO
```

### Comparing `dubo-0.2.4/LICENSE` & `dubo-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dubo-0.2.4/pyproject.toml` & `dubo-0.2.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [tool.poetry]
 name = "dubo"
-version = "0.2.4"
+version = "0.2.5"
 description = "Analytics made simple"
 authors = ["Andrew Duberstein <ajduberstein@gmail.com>", "Andrew Duberstein <duber@mercator.tech>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^1.0.0"
+altair = "^5.0.1"
+pydeck = "^0.8.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 black = "^22.12.0"
 pylint = "^2.15.9"
 jupyterlite = {version = "^0.1.0b17", allow-prereleases = true}
 jupyterlab-server = "^2.18.0"
```

### Comparing `dubo-0.2.4/setup.py` & `dubo-0.2.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['dubo']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pandas>=1.0.0,<2.0.0']
+['altair>=5.0.1,<6.0.0', 'pandas>=1.0.0,<2.0.0', 'pydeck>=0.8.0,<0.9.0']
 
 setup_kwargs = {
     'name': 'dubo',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'Analytics made simple',
     'long_description': 'dubo\n====\n\ndubo is a client for running LLMs against DataFrames and other 2D data.\n\nIt is currently in an alpha release and not yet ready for use in production pipelines.\n',
     'author': 'Andrew Duberstein',
     'author_email': 'ajduberstein@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dubo-0.2.4/PKG-INFO` & `dubo-0.2.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: dubo
-Version: 0.2.4
+Version: 0.2.5
 Summary: Analytics made simple
 License: MIT
 Author: Andrew Duberstein
 Author-email: ajduberstein@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: altair (>=5.0.1,<6.0.0)
 Requires-Dist: pandas (>=1.0.0,<2.0.0)
+Requires-Dist: pydeck (>=0.8.0,<0.9.0)
 Description-Content-Type: text/markdown
 
 dubo
 ====
 
 dubo is a client for running LLMs against DataFrames and other 2D data.
```

