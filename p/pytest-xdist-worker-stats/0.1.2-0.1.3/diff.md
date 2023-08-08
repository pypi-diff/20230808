# Comparing `tmp/pytest_xdist_worker_stats-0.1.2.tar.gz` & `tmp/pytest_xdist_worker_stats-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_xdist_worker_stats-0.1.2.tar", max compression
+gzip compressed data, was "pytest_xdist_worker_stats-0.1.3.tar", max compression
```

## Comparing `pytest_xdist_worker_stats-0.1.2.tar` & `pytest_xdist_worker_stats-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-06-15 08:53:33.817321 pytest_xdist_worker_stats-0.1.2/LICENSE
--rw-r--r--   0        0        0     2004 2023-06-15 08:57:34.823044 pytest_xdist_worker_stats-0.1.2/README.md
--rw-r--r--   0        0        0     2831 2023-06-19 16:09:38.510823 pytest_xdist_worker_stats-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       75 2023-06-19 16:09:38.510823 pytest_xdist_worker_stats-0.1.2/pytest_xdist_worker_stats/__init__.py
--rw-r--r--   0        0        0      937 2023-06-15 08:53:33.821321 pytest_xdist_worker_stats-0.1.2/pytest_xdist_worker_stats/options.py
--rw-r--r--   0        0        0     2333 2023-06-19 16:09:38.510823 pytest_xdist_worker_stats-0.1.2/pytest_xdist_worker_stats/plugin.py
--rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-08 21:24:46.749866 pytest_xdist_worker_stats-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2049 2023-08-08 21:24:46.749866 pytest_xdist_worker_stats-0.1.3/README.md
+-rw-r--r--   0        0        0     2860 2023-08-08 21:24:46.749866 pytest_xdist_worker_stats-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-08-08 21:24:46.749866 pytest_xdist_worker_stats-0.1.3/pytest_xdist_worker_stats/__init__.py
+-rw-r--r--   0        0        0      937 2023-08-08 21:24:46.749866 pytest_xdist_worker_stats-0.1.3/pytest_xdist_worker_stats/options.py
+-rw-r--r--   0        0        0     2333 2023-08-08 21:24:46.749866 pytest_xdist_worker_stats-0.1.3/pytest_xdist_worker_stats/plugin.py
+-rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.1.3/PKG-INFO
```

### Comparing `pytest_xdist_worker_stats-0.1.2/LICENSE` & `pytest_xdist_worker_stats-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.2/README.md` & `pytest_xdist_worker_stats-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pytest-xdist-worker-stats
 
-A pytest plugin
+A pytest plugin to list worker statistics after a xdist run.
 
 ## Installation
 
 ```shell
 $ pip install pytest-xdist-worker-stats
 ```
```

### Comparing `pytest_xdist_worker_stats-0.1.2/pyproject.toml` & `pytest_xdist_worker_stats-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-xdist-worker-stats"
-version = "0.1.2"
+version = "0.1.3"
 description = "A pytest plugin to list worker statistics after a xdist run."
 authors = ["Mikuláš Poul <mikulaspoul@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pytest_xdist_worker_stats"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -27,30 +27,31 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pytest = "^7.3.2"
 pytest-xdist = "^3.3.1"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-ruff = "^0.0.272"
+black = "^23.7.0"
+ruff = "^0.0.283"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
-target_version = ['py310']
+target_version = ['py310', 'py311', 'py312']
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

### Comparing `pytest_xdist_worker_stats-0.1.2/pytest_xdist_worker_stats/options.py` & `pytest_xdist_worker_stats-0.1.3/pytest_xdist_worker_stats/options.py`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.2/pytest_xdist_worker_stats/plugin.py` & `pytest_xdist_worker_stats-0.1.3/pytest_xdist_worker_stats/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.2/PKG-INFO` & `pytest_xdist_worker_stats-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xdist-worker-stats
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pytest plugin to list worker statistics after a xdist run.
 Home-page: https://github.com/mikicz/pytest-xdist-worker-stats
 License: MIT
 Keywords: pytest,xdist,pytest-xdist
 Author: Mikuláš Poul
 Author-email: mikulaspoul@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -21,15 +21,15 @@
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Requires-Dist: pytest-xdist (>=3.3.1,<4.0.0)
 Project-URL: Repository, https://github.com/mikicz/pytest-xdist-worker-stats
 Description-Content-Type: text/markdown
 
 # pytest-xdist-worker-stats
 
-A pytest plugin
+A pytest plugin to list worker statistics after a xdist run.
 
 ## Installation
 
 ```shell
 $ pip install pytest-xdist-worker-stats
 ```
```

