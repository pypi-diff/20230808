# Comparing `tmp/pytest_unused_fixtures-0.1.3.tar.gz` & `tmp/pytest_unused_fixtures-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_unused_fixtures-0.1.3.tar", max compression
+gzip compressed data, was "pytest_unused_fixtures-0.1.4.tar", max compression
```

## Comparing `pytest_unused_fixtures-0.1.3.tar` & `pytest_unused_fixtures-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-06-13 20:43:22.326631 pytest_unused_fixtures-0.1.3/LICENSE
--rw-r--r--   0        0        0     2233 2023-06-30 09:08:19.480730 pytest_unused_fixtures-0.1.3/README.md
--rw-r--r--   0        0        0     2799 2023-06-30 09:08:19.480730 pytest_unused_fixtures-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      153 2023-06-15 08:59:11.585729 pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/__init__.py
--rw-r--r--   0        0        0       88 2023-06-14 21:25:32.009991 pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/decorators.py
--rw-r--r--   0        0        0     1226 2023-06-30 09:08:19.480730 pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/options.py
--rw-r--r--   0        0        0     4543 2023-06-30 09:08:19.480730 pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/plugin.py
--rw-r--r--   0        0        0     1529 2023-06-30 09:08:19.480730 pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/xdist.py
--rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pytest_unused_fixtures-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2233 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/README.md
+-rw-r--r--   0        0        0     2881 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/__init__.py
+-rw-r--r--   0        0        0       88 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/decorators.py
+-rw-r--r--   0        0        0     1226 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/options.py
+-rw-r--r--   0        0        0     4543 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/plugin.py
+-rw-r--r--   0        0        0     1529 2023-08-08 21:32:08.732201 pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/xdist.py
+-rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pytest_unused_fixtures-0.1.4/PKG-INFO
```

### Comparing `pytest_unused_fixtures-0.1.3/LICENSE` & `pytest_unused_fixtures-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.3/README.md` & `pytest_unused_fixtures-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.3/pyproject.toml` & `pytest_unused_fixtures-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "pytest-unused-fixtures"
-version = "0.1.3"
+version = "0.1.4"
 description = "A pytest plugin to list unused fixtures after a test run."
 authors = ["Mikuláš Poul <mikulaspoul@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pytest_unused_fixtures"}]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Testing",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Framework :: Pytest",
 ]
 include = ["LICENSE"]
 repository = "https://github.com/mikicz/pytest-unused-fixtures"
@@ -26,31 +27,32 @@
 pytest-unused-fixtures = "pytest_unused_fixtures"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytest = "^7.3.2"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-ruff = "^0.0.272"
+black = "^23.7.0"
+ruff = "^0.0.283"
 pytest-xdist = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
-target_version = ['py310']
+target_version = ['py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
       \.git         # exclude a few common directories in the
-    | venv          # root of the project
+    | \.tox         # root of the project
+    | venv
   )/
 )
 '''
 
 
 [tool.ruff]
 select = [
```

### Comparing `pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/options.py` & `pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/options.py`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/plugin.py` & `pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.3/pytest_unused_fixtures/xdist.py` & `pytest_unused_fixtures-0.1.4/pytest_unused_fixtures/xdist.py`

 * *Files identical despite different names*

### Comparing `pytest_unused_fixtures-0.1.3/PKG-INFO` & `pytest_unused_fixtures-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-unused-fixtures
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pytest plugin to list unused fixtures after a test run.
 Home-page: https://github.com/mikicz/pytest-unused-fixtures
 License: MIT
 Keywords: pytest,fixtures
 Author: Mikuláš Poul
 Author-email: mikulaspoul@gmail.com
 Requires-Python: >=3.9,<4.0
```

