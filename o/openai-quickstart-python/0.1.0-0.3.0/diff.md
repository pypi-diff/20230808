# Comparing `tmp/openai_quickstart_python-0.1.0.tar.gz` & `tmp/openai_quickstart_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_quickstart_python-0.1.0.tar", max compression
+gzip compressed data, was "openai_quickstart_python-0.3.0.tar", max compression
```

## Comparing `openai_quickstart_python-0.1.0.tar` & `openai_quickstart_python-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-08-07 08:45:17.145343 openai_quickstart_python-0.1.0/LICENSE
--rw-r--r--   0        0        0     1210 2023-08-07 08:45:17.145343 openai_quickstart_python-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-08-08 10:29:07.625846 openai_quickstart_python-0.1.0/openai_quickstart_python/__init__.py
--rw-r--r--   0        0        0      973 2023-08-08 10:31:40.942461 openai_quickstart_python-0.1.0/openai_quickstart_python/app.py
--rw-r--r--   0        0        0     1746 2023-08-08 10:31:48.070491 openai_quickstart_python-0.1.0/openai_quickstart_python/static/dog.png
--rw-r--r--   0        0        0     1309 2023-08-08 10:31:48.070491 openai_quickstart_python-0.1.0/openai_quickstart_python/static/main.css
--rw-r--r--   0        0        0      597 2023-08-08 10:31:51.170504 openai_quickstart_python-0.1.0/openai_quickstart_python/templates/index.html
--rw-r--r--   0        0        0      846 2023-08-08 09:49:20.143645 openai_quickstart_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 openai_quickstart_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-07 08:45:17.145343 openai_quickstart_python-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1210 2023-08-07 08:45:17.145343 openai_quickstart_python-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-08 10:29:07.625846 openai_quickstart_python-0.3.0/openai_quickstart_python/__init__.py
+-rw-r--r--   0        0        0      973 2023-08-08 10:31:40.942461 openai_quickstart_python-0.3.0/openai_quickstart_python/app.py
+-rw-r--r--   0        0        0     1746 2023-08-08 10:31:48.070491 openai_quickstart_python-0.3.0/openai_quickstart_python/static/dog.png
+-rw-r--r--   0        0        0     1309 2023-08-08 10:31:48.070491 openai_quickstart_python-0.3.0/openai_quickstart_python/static/main.css
+-rw-r--r--   0        0        0      597 2023-08-08 10:31:51.170504 openai_quickstart_python-0.3.0/openai_quickstart_python/templates/index.html
+-rw-r--r--   0        0        0      932 2023-08-08 11:56:24.662531 openai_quickstart_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 openai_quickstart_python-0.3.0/PKG-INFO
```

### Comparing `openai_quickstart_python-0.1.0/LICENSE` & `openai_quickstart_python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_quickstart_python-0.1.0/README.md` & `openai_quickstart_python-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `openai_quickstart_python-0.1.0/openai_quickstart_python/app.py` & `openai_quickstart_python-0.3.0/openai_quickstart_python/app.py`

 * *Files identical despite different names*

### Comparing `openai_quickstart_python-0.1.0/openai_quickstart_python/static/dog.png` & `openai_quickstart_python-0.3.0/openai_quickstart_python/static/dog.png`

 * *Files identical despite different names*

### Comparing `openai_quickstart_python-0.1.0/openai_quickstart_python/static/main.css` & `openai_quickstart_python-0.3.0/openai_quickstart_python/static/main.css`

 * *Files identical despite different names*

### Comparing `openai_quickstart_python-0.1.0/openai_quickstart_python/templates/index.html` & `openai_quickstart_python-0.3.0/openai_quickstart_python/templates/index.html`

 * *Files identical despite different names*

### Comparing `openai_quickstart_python-0.1.0/pyproject.toml` & `openai_quickstart_python-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-quickstart-python"
-version = "0.1.0"
+version = "0.3.0"
 description = "qualcosa  da  dichiarare come  descrizione"
 authors = ["flavio <flavio.joshua@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_quickstart_python"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -29,11 +29,13 @@
 requests = "2.26.0"
 six = "1.16.0"
 toml = "0.10.2"
 tqdm = "4.62.3"
 urllib3 = "1.26.7"
 werkzeug = "2.0.2"
 
+[tool.poetry.scripts]
+openai-quickstart-python = 'openai_quickstart_python.main:main'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openai_quickstart_python-0.1.0/PKG-INFO` & `openai_quickstart_python-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-quickstart-python
-Version: 0.1.0
+Version: 0.3.0
 Summary: qualcosa  da  dichiarare come  descrizione
 Author: flavio
 Author-email: flavio.joshua@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

